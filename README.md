# p5-debian-firmware-custom-dell_g7_17
Custom missing DELL G7 17 firmware for Debian GNU/Linux.

This package should fix:
```
W: Possible missing firmware /lib/firmware/rtl_nic/rtl8168fp-3.fw for module r8169
W: Possible missing firmware /lib/firmware/i915/icl_dmc_ver1_09.bin for module i915
W: Possible missing firmware /lib/firmware/i915/skl_huc_2.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/bxt_huc_2.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/kbl_huc_4.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/glk_huc_4.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/kbl_huc_4.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/cml_huc_4.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/cml_guc_33.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/icl_huc_9.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/ehl_huc_9.0.0.bin for module i915
W: Possible missing firmware /lib/firmware/i915/ehl_guc_33.0.4.bin for module i915
W: Possible missing firmware /lib/firmware/i915/tgl_huc_7.0.3.bin for module i915
W: Possible missing firmware /lib/firmware/i915/tgl_guc_35.2.0.bin for module i915
```

You can make your own configuration based on this package. It's simple - Just modify CMakeLists.txt. =)

## download release debian package
[Download debian package here](../../releases/latest)

## build
`$ cmake ${path_to_source} && cpack -G DEB`

## install
`# apt install ./p5-firmware-custom-dell_g7_17_${version}_all.deb`
