# WL-WN53A8A

## /target/linux/bcm53xx/image/Makefile
~~~
Ligne 461
define Device/phicomm_k3
  DEVICE_VENDOR := PHICOMM
  DEVICE_MODEL := K3
  DEVICE_PACKAGES := $(BRCMFMAC_4366C0) $(USB3_PACKAGES)
  IMAGES := trx
endef
TARGET_DEVICES += phicomm_k3
~~~

## /target/linux/bcm53xx/base-files/etc/board.d
~~~
ligne 35
bcm53xx_setup_interfaces()
{
	phicomm,k3)
		ucidef_set_interfaces_lan_wan "lan1 lan2 lan3" "wan"
		;;
}
~~~
