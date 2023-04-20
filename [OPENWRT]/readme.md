# OPENWRT

https://openwrt.org/docs/guide-developer/source-code/start

### Structure générale de la source
Ce sont les dossiers que vous pouvez trouver dans le git du projet:

    /config : fichiers de configuration pour menuconfig
    /inclure : fichiers de configuration de makefile
    /paquet : packages makefile et configuration
    /scripts : scripts divers utilisés tout au long du processus de construction
    /cible : makefile et configuration pour la construction d'image builder, kernel, sdk et la chaîne d'outils construite par buildroot.
    /chaîne à outils : makefile et configuration pour la construction de la chaîne d'outils
    /outils : divers outils utilisés tout au long du processus de construction

## Prise en charge 
https://downloads.openwrt.org/

## HELIOS64

##Fichiers importants
Il s'agit d'une carte générale de l'emplacement des fichiers les plus importants:

### /target/linux/< arch_name >/base-files/etc/…
Ce dossier contient des fichiers et des dossiers qui seront intégrés dans le dossier / etc du firmware.

##Ce sont ses sous-dossiers et fichiers:

### …board.d/ 
scripts pour définir le matériel par défaut spécifique à l'appareil, comme les leds et les interfaces réseau.
### …hotplug.d/ 
scripts pour définir les actions spécifiques à l'appareil à effectuer automatiquement lors du hotpluging des appareils
### …init.d/ 
scripts pour définir des actions spécifiques à l'appareil à effectuer automatiquement au démarrage
### …uci-défauts/ 
fichiers pour définir les valeurs par défaut de configuration uci spécifiques au périphérique
### …diag.sh 
définit ce que led à utiliser pour les codes d'erreur pour chaque carte

##Notez que certaines de ces fonctions sont maintenant effectuées dans le DTS pour la carte.

### /target/linux/< arch_name >/base-files/lib/…
Ce dossier contient des fichiers et des dossiers qui seront intégrés dans le dossier / lib du firmware.

## Ce sont ses sous-dossiers et fichiers:

### …< arch_name >.sh 
nom complet du tableau lisible par l'homme associé au nom du tableau sûr du script

### …preinit/ < arch_name > 
scripts de démarrage préinit

### …Mise à niveau/ 
scripts de mise à niveau courants < arch_name >

### /target/linux/< arch_name >/base-files/sbin
Ce dossier contient des fichiers et des dossiers qui seront intégrés dans le dossier / sbin du firmware, généralement des scripts et outils courants < arch_name > sbin.

### /target/linux/< arch_name >/dts/
Appareil des fichiers source d'arborescence ou dts pour faire court.

### Certaines architectures ont le répertoire DTS plus bas. Les appareils ARM, par exemple, l'ont généralement localisé à files-X.yy/arch/arm/boot/dts/

Si le fichier DTS ou DTSI est déjà présent dans Linux en amont, il ne sera généralement pas présent dans la source OpenWrt. 

Configuration de la cible et exécution make target/linux/{clean,prepare} téléchargera et corrigera Linux, permettant de trouver le fichier résultant dans le build_dir

/target/linux/< arch_name >/image/
Configuration nécessaire pour créer des images flashables spécifiques à l'appareil.

/target/linux/< arch_name >/< board_name >/
Configuration spécifique au forum.

/target/linux / < arch_name > / modules.mk
Fichier de configuration du module du noyau spécifique à l'arche pour menuconfig





## WL-WN538A8

