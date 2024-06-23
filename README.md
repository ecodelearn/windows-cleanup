# windows-cleanup

# Comandos para reparar arquivos de sistema corrompidos

## Os comandos devem ser executados um por um

Abra um terminal cmd.exe como Administrador e execute um de cada vez na mesma janela.
```plain text
DISM.exe /Online /Cleanup-image /Restorehealth

sfc /scannow

DISM /Online /Cleanup-Image /StartComponentCleanup
```
