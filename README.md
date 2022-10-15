# New World tools

## Downloads

Download the compiled binaries in [Releases](https://github.com/new-world-tools/new-world-tools/releases)

## Usage

### Pak extracter

Powershell:
```powershell
.\pak-extracter.exe `
    -assets "C:\Program Files (x86)\Steam\steamapps\common\New World\assets" `
    -output ".\extract"
```

Optional:
```powershell
    -threads 3 `
    -filter .ext1,.ext2 `
    -decompress-azcs `
    -hash ".\extract\files.sha1"
```

### Datasheet converter

Supported formats are `csv` (default) and `json`

Powershell:
```powershell
.\datasheet-converter.exe `
    -input ".\extract\sharedassets\springboardentitites\datatables" `
    -output ".\extract\datasheets" `
    -format csv
```

Optional:
```powershell
    -threads 3 `
    -localization ".\extract\localization\en-us"
```
