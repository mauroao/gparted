
# Projeto SSD

Espetar do lado do cabo de rede
F2 + F8

Comandos e ferramentas:

- DD
- BalenaEtcher
- GParted - Live USB ← Rufus?
```
sudo smartctl -i /dev/nvme0n1
```
Partition - Resize:
```
sudo dd if=/dev/nvme of=/dev/nvme bs=1M status=progress
```
Erros:
- Invalid Argument
- Backup partition at the end of drive
```
sudo gdisk /dev/nvme
```
Warning! One or more CRC don't match

Opções do gdisk:

- X - Expert
- E - Relocate backup data
- W - Write
- Y - Yes

lsblk

1949
