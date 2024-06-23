## windows-cleanup

### Comandos para reparar arquivos de sistema corrompidos

### Os comandos devem ser executados um por um

Abra um terminal cmd.exe como Administrador e execute um de cada vez na mesma janela.
```plain text
DISM.exe /Online /Cleanup-image /Restorehealth

sfc /scannow

DISM /Online /Cleanup-Image /StartComponentCleanup
```


Atualização de programas na linha de comando do PowerShell usando WinGet.
A ferramenta de linha de comando winget só tem suporte no Windows 10 1709 (build 16299) ou posterior neste momento.


```plain text
Add-AppxPackage -RegisterByFamilyName -MainPackage Microsoft.DesktopAppInstaller_8wekyb3d8bbwe
```

```plain text
winget.exe upgrade -i --all --include-unknown
```
Ativando Virtualização de Máquina
```plain text
Set-VMProcessor -VMName <VMName> -ExposeVirtualizationExtensions $true
Update-VMVersion -VMName <VMName>
```
Ativando Sandbox
```plain text
Enable-WindowsOptionalFeature -FeatureName "Containers-DisposableClientVM" -All -Online
```
Consultar para mais explicações e atualização deste Readme.
```plain text
https://learn.microsoft.com/pt-br/windows/security/application-security/application-isolation/windows-sandbox/windows-sandbox-configure-using-wsb-file#networking
```
