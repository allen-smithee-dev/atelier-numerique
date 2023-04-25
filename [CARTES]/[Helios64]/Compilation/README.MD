# dossier de compilation 
EXEMPLE:

## mkdir /COMPILATION/ && cd /COMPILATION/

### Script - Assembleur  || script des compilations bootloader / firmware / image 
git clone -b branch https://github.com/name/repo.git
### Prise en charge - Board  ||  ajout specifique 
git clone -b branch https://github.com/name/repo.git
### Linux - Kernel  || prise en charge materiel
git clone -b branch https://github.com/name/repo.git
### Firmware ARM - Rkbin  ||  microcode architecture
git clone -b branch https://github.com/name/repo.git
### Distribution linux pour la compilation - Station  ||  distribution X86
git clone -b branch https://github.com/name/repo.git
### Lanceur - U-boot  ||   Bootloader
git clone -b branch https://github.com/name/repo.git

## mkdir /COMPILATION/DISTRIBUTION && cd /COMPILATION/DISTRIBUTION/
### Distribution - Build  || Distribution associe
git clone -b branch https://github.com/name/repo.git

~~~
/COMPILATION
├── Assembleur/
├── Board/
├── DISTRIBUTION/
├── Kernel/
├── Rkbin/
├── Station/
└── U-boot/
~~~
