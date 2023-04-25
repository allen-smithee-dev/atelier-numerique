# dossier de compilation 

EXEMPLE:

## mkdir /COMPILATION/RK3399/HELIOS64 && cd /COMPILATION/RK3399/HELIOS64/
### Firmware ARM - Rkbin
git clone -b branch https://github.com/name/repo.git
### Lanceur - U-boot
git clone -b branch https://github.com/name/repo.git
### Linux - Kernel
git clone -b branch https://github.com/name/repo.git

## mkdir /COMPILATION/RK3399/HELIOS64/DISTRIBUTION && cd /COMPILATION/RK3399/HELIOS64/DISTRIBUTION/
### Distribution - Build
git clone -b branch https://github.com/name/repo.git
~~~
ll /COMPILATION/RK3399/HELIOS64/
├── DISTRIBUTION/DISTRIBUTION/Build
├── Kernel/
├── Rkbin/
└── U-boot/
~~~

# SCRIPT de compilation
