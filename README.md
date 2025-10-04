# 👻 Ghost Nchekwa Module
**PowerShell-dabere na Windows na Azure Nchekwa Mgbakwunye Ngwá ọrụ**

> **Nchekwa mgbakwunye na-arụ ọrụ maka Windows njedebe ebe na Azure gburugburu.** Ghost na-enye PowerShell-dabere mgbakwunye ọrụ ndị nwere ike inye aka ibelata ọtụtụ mwakpo vectors site na imechi ọrụ na protocols na-adịghị mkpa.

## ⚠️ Mkpa Mkpesa Mkpọchi

**NNWALE DỊ MKPa**: Nnwalee Ghost mgbe niile na mbụ na gburugburu na-abụghị mmepụta. Imechi ọrụ nwere ike imetụta ọrụ azụmaahịa ziri ezi.

**ENWEGHỊ EKWENYE**: Ọ bụ ezie na Ghost na-elekwasị anya na ọtụtụ mwakpo vectors, enweghị ngwá ọrụ nchekwa pụrụ igbochi mwakpo niile. Nke a bụ otu akụkụ nke atụmatụ nchekwa zuru ezu.

**MMETỤTA ỌRỤ**: Ụfọdụ ọrụ nwere ike imetụta ọrụ sistemu. Nyochaa nke ọma nhazi ọ bụla tupu ịmalite.

**NYOCHA ỌKACHAMARA**: Maka gburugburu mmepụta, kparịta ụka na ndị ọkachamara nchekwa iji hụ na nhazi na-adaba na mkpa nke nzukọ gị.

## 📊 Nchekwa Landscape

Mmebi Ransomware ruru **$57 billion na 2025**, nyocha na-egosi na ọtụtụ mwakpo ga-aga nke ọma na-eji ọrụ Windows bụ isi na nhazi ọjọọ. Ọtụtụ mwakpo vectors gụnyere:

- **90% nke ransomware ihe omume** gụnyere RDP nrigbu
- **SMBv1 adịghị ike** kwere ka mwakpo dị ka WannaCry na NotPetya
- **Akwụkwọ macros** ka bụ isi malware nnyefe usoro
- **USB-dabere mwakpo** na-aga n'ihu ịlụso ikuku-oghere netwọk ọgụ
- **PowerShell ọjọọ ojiji** amụbaala nke ukwuu n'afọ ndị gara aga

## 🛡️ Ghost Nchekwa Ọrụ

Ghost na-enye **16 Windows mgbakwunye ọrụ** gbakwunyere **Azure nchekwa ijikọ**:

### Windows Endpoint Mgbakwunye

| Ọrụ | Ebumnuche | Ntụle |
|----------|---------|----------------|
| `Set-RDP` | Na-achịkwa Remote Desktop nnweta | Nwere ike imetụta nchịkwa dị anya |
| `Set-SMBv1` | Na-achịkwa ochie SMB protocol | Achọrọ maka sistemu ochie |
| `Set-AutoRun` | Na-achịkwa AutoPlay/AutoRun | Nwere ike imetụta mfe onye ọrụ |
| `Set-USBStorage` | Na-amachi USB nchekwa ngwaọrụ | Nwere ike imetụta iji USB ziri ezi |
| `Set-Macros` | Na-achịkwa Office macro mmezu | Nwere ike imetụta akwụkwọ macro-kwere |
| `Set-PSRemoting` | Na-achịkwa PowerShell remoting | Nwere ike imetụta nchịkwa dị anya |
| `Set-WinRM` | Na-achịkwa Windows Remote Management | Nwere ike imetụta nchịkwa dị anya |
| `Set-LLMNR` | Na-achịkwa aha mkpebi protocol | Ọ na-adịkarị mma ime ka ọ ghara ịrụ ọrụ |
| `Set-NetBIOS` | Na-achịkwa NetBIOS na TCP/IP | Nwere ike imetụta ngwa ochie |
| `Set-AdminShares` | Na-achịkwa nchịkwa shares | Nwere ike imetụta nnweta faịlụ dị anya |
| `Set-Telemetry` | Na-achịkwa nchịkọta data | Nwere ike imetụta ike nyocha |
| `Set-GuestAccount` | Na-achịkwa akaụntụ ndị ọbịa | Ọ na-adịkarị mma ime ka ọ ghara ịrụ ọrụ |
| `Set-ICMP` | Na-achịkwa ping nzaghachi | Nwere ike imetụta nyocha netwọk |
| `Set-RemoteAssistance` | Na-achịkwa Enyemaka Dị Anya | Nwere ike imetụta ọrụ helpdesk |
| `Set-NetworkDiscovery` | Na-achịkwa nchọpụta netwọk | Nwere ike imetụta ịchọgharị netwọk |
| `Set-Firewall` | Na-achịkwa Windows Firewall | Dị mkpa maka nchekwa netwọk |

### Azure Cloud Nchekwa

| Ọrụ | Ebumnuche | Ihe achọrọ |
|----------|---------|--------------|
| `Set-AzureSecurityDefaults` | Na-eme ka Azure AD nchekwa bụ isi | Microsoft Graph ikike |
| `Set-AzureConditionalAccess` | Na-ahazi amụma nnweta | Azure AD P1/P2 ikikere |
| `Set-AzurePrivilegedUsers` | Na-enyocha akaụntụ nwere ikike pụrụ iche | Global Admin ikike |

### Nhọrọ Mbugharị Enterprise

| Ụzọ | Okwu Ojiji | Ihe achọrọ |
|--------|----------|--------------|
| **Omenala Kpọmkwem** | Nnwale, obere gburugburu | Ikike nchịkwa mpaghara |
| **Group Policy** | Gburugburu ngalaba | Nchịkwa ngalaba, njikwa GP |
| **Microsoft Intune** | Ngwaọrụ igwe ojii na-achịkwa | Ikikere Intune, Graph API |

## 🚀 Mmalite Ngwa Ngwa

### Nyocha Nchekwa
```powershell
# Bukota Ghost module
IEX(Invoke-WebRequest 'https://raw.githubusercontent.com/jimrtyler/Ghost/main/Ghost.ps1')

# Chọpụta ọnọdụ nchekwa ugbu a
Get-Ghost
```

### Mgbakwunye Bụ Isi (Nwalee Mbụ)
```powershell
# Mgbakwunye dị mkpa - nwalee na gburugburu ụlọ nyocha mbụ
Set-Ghost -SMBv1 -AutoRun -Macros

# Nyochaa mgbanwe
Get-Ghost
```

### Mbugharị Enterprise
```powershell
# Mbugharị Group Policy (gburugburu ngalaba)
Set-Ghost -SMBv1 -AutoRun -GroupPolicy

# Mbugharị Intune (ngwaọrụ igwe ojii na-achịkwa)
Set-Ghost -SMBv1 -RDP -USBStorage -Intune
```

## 📋 Ụzọ Nwụnye

### Nhọrọ 1: Nbudata Ozugbo (Nnwale)
```powershell
IEX(Invoke-WebRequest 'https://raw.githubusercontent.com/jimrtyler/Ghost/main/Ghost.ps1')
```

### Nhọrọ 2: Nwụnye Module
```powershell
# Wụnye site na PowerShell Gallery (mgbe ọ dị)
Install-Module Ghost -Scope CurrentUser
Import-Module Ghost
```

### Nhọrọ 3: Mbugharị Enterprise
```powershell
# Depụta na ebe netwọk maka mbugharị Group Policy
# Hazie Intune PowerShell scripts maka mbugharị igwe ojii
```

## 💼 Ihe Atụ Okwu Ojiji

### Obere Azụmaahịa
```powershell
# Nchekwa bụ isi na mmetụta kacha nta
Set-Ghost -SMBv1 -AutoRun -Macros -ICMP
```

### Gburugburu Nlekọta Ahụike
```powershell
# Mgbakwunye lekwasịrị anya na HIPAA
Set-Ghost -SMBv1 -RDP -USBStorage -AdminShares -Telemetry
```

### Ọrụ Ego
```powershell
# Nhazi nchekwa dị elu
Set-Ghost -RDP -SMBv1 -AutoRun -USBStorage -Macros -PSRemoting -AdminShares
```

### Nzukọ Cloud-Mbụ
```powershell
# Mbugharị Intune-achịkwa
Connect-IntuneGhost -Interactive
Set-Ghost -SMBv1 -RDP -AutoRun -Macros -Intune
```

## 🔍 Nkọwa Ọrụ

### Ọrụ Mgbakwunye Bụ Isi

#### Ọrụ Netwọk
- **RDP**: Na-egbochi nnweta desktop dị anya ma ọ bụ na-eme ka ọdụ ụgbọ mmiri ghara ịdị n'usoro
- **SMBv1**: Na-eme ka protocol ịkekọrịta faịlụ ochie ghara ịrụ ọrụ
- **ICMP**: Na-egbochi nzaghachi ping maka nyocha
- **LLMNR/NetBIOS**: Na-egbochi protocols mkpebi aha ochie

#### Nchekwa Ngwa
- **Macros**: Na-eme ka mmezu macro na ngwa Office ghara ịrụ ọrụ
- **AutoRun**: Na-egbochi mmezu akpaaka site na media ewepụrụ ewepụ

#### Nchịkwa Dị Anya
- **PSRemoting**: Na-eme ka nnọkọ PowerShell dị anya ghara ịrụ ọrụ
- **WinRM**: Na-akwụsị Windows Remote Management
- **Remote Assistance**: Na-egbochi njikọ enyemaka dị anya

#### Nchịkwa Nnweta
- **Admin Shares**: Na-eme ka C$, ADMIN$ shares ghara ịrụ ọrụ
- **Guest Account**: Na-eme ka nnweta akaụntụ ndị ọbịa ghara ịrụ ọrụ
- **USB Storage**: Na-amachi ojiji ngwaọrụ USB

### Njikọ Azure
```powershell
# Jikọọ na Azure tenant
Connect-AzureGhost -Interactive

# Mee ka nchekwa defaults rụọ ọrụ
Set-AzureSecurityDefaults -Enable

# Hazie nnweta nke nwere ọnọdụ
Set-AzureConditionalAccess -BlockLegacyAuth -RequireMFA

# Nyochaa ndị ọrụ nwere ikike pụrụ iche
Set-AzurePrivilegedUsers -AuditOnly
```

### Njikọ Intune (Ọhụrụ na v2)
```powershell
# Jikọọ na Intune
Connect-IntuneGhost -Interactive

# Bugharịa site na amụma Intune
Set-IntuneGhost -Settings @{
    RDP = $true
    SMBv1 = $true
    USBStorage = $true
    Macros = $true
}
```

## ⚠️ Ntụle Dị Mkpa

### Ihe Achọrọ Nnwale
- **Gburugburu Ụlọ Nyocha**: Nwalee nhazi niile na gburugburu kewapụrụ ekewa mbụ
- **Mbugharị Nkeji Nkeji**: Gbasaa nwayọọ nwayọọ iji chọpụta nsogbu
- **Atụmatụ Nlaghachi**: Hụ na ị nwere ike ịlaghachi mgbanwe ma ọ bụrụ na achọrọ ya
- **Akwụkwọ**: Dekọọ nhazi ndị na-arụ ọrụ maka gburugburu gị

### Mmetụta Nwere Ike
- **Arụpụta Onye Ọrụ**: Ụfọdụ nhazi nwere ike imetụta usoro ọrụ kwa ụbọchị
- **Ngwa Ochie**: Sistemu ochie nwere ike chọọ protocols ụfọdụ
- **Nnweta Dị Anya**: Tụlee mmetụta na nchịkwa dị anya ziri ezi
- **Usoro Azụmaahịa**: Chọpụta na nhazi anaghị emebi ọrụ dị mkpa

### Njedebe Nchekwa
- **Nchekwa Miri Emi**: Ghost bụ otu akụkụ nchekwa, ọbụghị ihe ngwọta zuru ezu
- **Nchịkwa Na-aga N'ihu**: Nchekwa chọrọ nleba anya na mmelite na-aga n'ihu
- **Ọzụzụ Onye Ọrụ**: Njikwa nka kwesịrị ịgakọta na nghọta nchekwa
- **Mgbanwe Iyi Egwu**: Ụzọ mwakpo ọhụrụ nwere ike gafere nchekwa ugbu a

## 🎯 Ihe Atụ Ọnọdụ Mwakpo

Ọ bụ ezie na Ghost na-elekwasị anya na ọtụtụ mwakpo vectors, mgbochi kpọmkwem dabere na mmezu kwesịrị ekwesị na nnwale:

### Mwakpo Ụdị WannaCry
- **Belata**: `Set-Ghost -SMBv1` na-eme ka protocol adịghị ike ghara ịrụ ọrụ
- **Ntụle**: Hụ na ọ dịghị sistemu ochie chọrọ SMBv1

### Ransomware Dabere na RDP
- **Belata**: `Set-Ghost -RDP` na-egbochi nnweta desktop dị anya
- **Ntụle**: Ọ nwere ike chọọ ụzọ nnweta dị anya ọzọ

### Malware Dabere na Akwụkwọ
- **Belata**: `Set-Ghost -Macros` na-eme ka mmezu macro ghara ịrụ ọrụ
- **Ntụle**: Nwere ike imetụta akwụkwọ macro-kwere ziri ezi

### Iyi Egwu E zipụrụ na USB
- **Belata**: `Set-Ghost -USBStorage -AutoRun` na-amachi ọrụ USB
- **Ntụle**: Nwere ike imetụta ojiji ngwaọrụ USB ziri ezi

## 🏢 Njirimara Enterprise

### Nkwado Group Policy
```powershell
# Tinye nhazi site na Group Policy registry
Set-Ghost -SMBv1 -RDP -AutoRun -GroupPolicy

# Nhazi na-emetụta ngalaba niile mgbe GP nwetagharị gasịrị
gpupdate /force
```

### Njikọ Microsoft Intune
```powershell
# Mepụta amụma Intune maka nhazi Ghost
Set-IntuneGhost -Settings $GhostSettings -Interactive

# Amụma na-ebugharị na ngwaọrụ ejikwa akpaaka
```

### Akụkọ Nrube Isi
```powershell
# Mepụta akụkọ nyocha nchekwa
Get-Ghost | Export-Csv -Path "Nyocha-Nchekwa-$(Get-Date -Format 'yyyy-MM-dd').csv"

# Akụkọ ọnọdụ nchekwa Azure
Get-AzureGhost | Out-File "Akụkọ-Nchekwa-Azure.txt"
```

## 📚 Omume Kacha Mma

### Tupu Mbugharị
1. **Akwụkwọ Ọnọdụ Ugbu A**: Gbaa `Get-Ghost` tupu mgbanwe
2. **Nwalee Nke Ọma**: Kwado na gburugburu na-abụghị mmepụta
3. **Atụmatụ Nlaghachi**: Mara ka esi alaghachi nhazi ọ bụla
4. **Nyocha Ndị Nwere Ọṅụṅụ**: Hụ na ngalaba azụmaahịa kwadoro mgbanwe

### N'oge Mbugharị
1. **Ụzọ Nkeji Nkeji**: Bugharịa na otu ndị pilot mbụ
2. **Leba Anya Mmetụta**: Lee mkpesa ndị ọrụ ma ọ bụ nsogbu sistemu
3. **Akwụkwọ Nsogbu**: Dekọọ nsogbu ọ bụla maka nrụtụ aka n'ọdịnihu
4. **Kọmụnikeshọn Mgbanwe**: Gwa ndị ọrụ banyere nkwalite nchekwa

### Mgbe Mbugharị Gasịrị
1. **Nyocha Mgbe Niile**: Gbaa `Get-Ghost` oge ụfọdụ iji kwado nhazi
2. **Melite Akwụkwọ**: Debe nhazi nchekwa ka ọ bụrụ nke ọhụrụ
3. **Nyochaa Ịdị Irè**: Lebaa anya ihe omume nchekwa
4. **Nkwalite Na-aga N'ihu**: Doziekwa nhazi dabere na ọnọdụ iyi egwu

## 🔧 Idozi Nsogbu

### Nsogbu Nkịtị
- **Mperi Ikike**: Hụ na nnọkọ PowerShell dị elu
- **Ndabere Ọrụ**: Ụfọdụ ọrụ nwere ike inwe ndabere
- **Nkwekọrịta Ngwa**: Nwalee ya na ngwa azụmaahịa
- **Njikọ Netwọk**: Kwado na nnweta dị anya ka na-arụ ọrụ

### Nhọrọ Mgbake
```powershell
# Mee ka ọrụ ụfọdụ rụọ ọrụ ọzọ ma ọ bụrụ na achọrọ ya
Set-RDP -Enable
Set-SMBv1 -Enable
Set-AutoRun -Enable
Set-Macros -Enable
```

## 👨‍💻 Banyere Onye Dere Ya

**Jim Tyler** - Microsoft MVP maka PowerShell
- **YouTube**: [@PowerShellEngineer](https://youtube.com/@PowerShellEngineer) (10,000+ ndị debanye aha)
- **Akwụkwọ Akụkọ**: [PowerShell.News](https://powershell.news) - Ọgụgụ isi nchekwa kwa izu
- **Onye Dere**: "PowerShell for Systems Engineers"
- **Ahụmahụ**: Ọtụtụ afọ iri nke PowerShell automation na nchekwa Windows

## 📄 Ikikere na Mkpọchi Ọrụ

### Ikikere MIT
A na-enye Ghost n'okpuru Ikikere MIT maka ojiji efu, mgbanwe na nkesa.

### Mkpọchi Ọrụ Nchekwa
- **Enweghị Ekwenye**: A na-enye Ghost "ka ọ dị" na-enweghị ekwenye ụdị ọ bụla
- **Nnwale Dị Mkpa**: Nwalee mgbe niile na gburugburu na-abụghị mmepụta mbụ
- **Nduzi Ọkachamara**: Kparịta ụka na ndị ọkachamara nchekwa maka mbugharị mmepụta
- **Mmetụta Ọrụ**: Ndị dere ya anaghị ahụ maka nkwụsị ọrụ ọ bụla
- **Nchekwa Zuru Ezu**: Ghost bụ akụkụ nke atụmatụ nchekwa zuru ezu

### Nkwado
- **GitHub Issues**: [Kọọ bug ma ọ bụ rịọọ njirimara](https://github.com/jimrtyler/Ghost/issues)
- **Akwụkwọ**: Jiri `Get-Help <function> -Full` maka enyemaka zuru ezu
- **Obodo**: PowerShell na nchekwa obodo forums

---

**🔒 Kwalite ọnọdụ nchekwa gị na Ghost - mana nwalee mgbe niile mbụ.**

```powershell
# Malite na nyocha, ọbụghị echiche
Get-Ghost
```

**⭐ Nye repository a kpakpando ma ọ bụrụ na Ghost na-enyere aka melite ọnọdụ nchekwa gị!**