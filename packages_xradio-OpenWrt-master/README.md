# Пакет xradio для OpenWrt-master_kernel-4.19:
* Дрaйвер wifi радиомодуля: xr819
* пакет подтянет все зависимости во время зборки..

* Поместить add-patch_dts_file-wifi-xradio.patch в любую директорию, в данном случае /home/user/zero
* и дать команду:
```
patch -p1 < ~/zero/add-patch_dts_file-wifi-xradio.patch
```

* Compile
```
./scripts/feeds update -a
./scripts/feeds install -a
make menuconfig
make V=s
```

