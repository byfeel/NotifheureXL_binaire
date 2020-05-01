# NotifheureXL_binaire
fichiers compilés pour le NotifheureXL


VERSION : 0.9.2 FIRMWARE  / 0.9 SPIFFS

Choisir le firmware , en fonction du type de matrice utilisé .

Matrice type FC16 : notifheurexl_FC16_numeroversion.bin
Matrice type ICStation :  notifheurexl_ICS_numeroversion.bin
Pour le dossier data, comprenant le serveur WEB, les fichiers de configurations et sauvegarde du notifheureXL , il faut utiliser le fichier :
notifheurexl_SPIFFS_numeroversion.bin

**flash**  
Mac / linux  
esptool.py --port /dev/tty.nonduport write_flash -fm dio 0x00000 notifheureXL_ICS_0.x.x.x.bin 0x300000 notifheureXL_SPIFFS_0.x.bin  

Windows  
esptool.py --port com6 write_flash -fm dio 0x00000 notifheureXL_ICS_0.x.x.x.bin 0x300000 notifheureXL_SPIFFS_0.x.bin

