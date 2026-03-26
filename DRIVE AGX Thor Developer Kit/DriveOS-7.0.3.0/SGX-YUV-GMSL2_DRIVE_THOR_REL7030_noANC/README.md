#### DriveOS version

* DriveOS: 7.0.3.0

#### Supported camera list
* SG2-AR0233C-5200-G2A-HXXX
* SG2-IMX390C-5300-GMSL2-HXXX
* SG5-IMX490C-5300-GMSL2-HXXX
* SG8S-AR0820C-5300-G2A-HXXX
* SG8-OX08DC-5300-_G2G-HXXX

#### Quick Start

1.Camera Port

```
Port1: Deser-E MAX96724: CSI-GH
Port2: Deser-D MAX96712: CSI-EF
Port3: Deser-C MAX96724: CSI-D
Port4: Deser-A MAX96724: CSI-AB
Port5: Deser-B MAX96792A: CSI-C
```

2.Install Driver

```
$ sudo rm -rf /usr/lib/nvsipl_drv/*
$ sudo cp -arf *.so /usr/lib/nvsipl_drv/
$ sudo cp libnvsipl_devblk_drv_deser_max96724.so /lib/
$ sudo cp libnvsipl_devblk_drv_deser_max96712_nv.so /lib/
```

3.Show FPS

3.1 SG2-AR0233C-5200-G2A-HXXX

```
# For Port1,link0
$ ./nvsipl_camera -c SG2_AR0233C_5200_G2A_96724_CPHY_x4 -m '0x0000 0x0000 0x0000 0x0001' -R -0 -1 -2 -s

# For Port2,link0
$ ./nvsipl_camera -c SG2_AR0233C_5200_G2A_CPHY_x4 -m '0x0000 0x0000 0x0001 0x0000' -R -0 -1 -2 -s

# For Port3,link0
$ ./nvsipl_camera -c SG2_AR0233C_5200_G2A_96724_CPHY_x4 -m '0x0000 0x0001 0x0000 0x0000' -R -0 -1 -2 -s

# For Port4,link0
$ ./nvsipl_camera -c SG2_AR0233C_5200_G2A_96724_CPHY_x4 -m '0x0001 0x0000 0x0000 0x0000' -R -0 -1 -2 -s
```

3.2 SG2-IMX390C-5300-GMSL2-HXXX

```
# For Port1,link0
$ ./nvsipl_camera -c SG2_IMX390C_5300_GMSL2_96724_CPHY_x4 -m '0x0000 0x0000 0x0000 0x0001' -R -0 -1 -2 -s

# For Port2,link0
$ ./nvsipl_camera -c SG2_IMX390C_5300_GMSL2_CPHY_x4 -m '0x0000 0x0000 0x0001 0x0000' -R -0 -1 -2 -s

# For Port3,link0
$ ./nvsipl_camera -c SG2_IMX390C_5300_GMSL2_96724_CPHY_x4 -m '0x0000 0x0001 0x0000 0x0000' -R -0 -1 -2 -s

# For Port4,link0
$ ./nvsipl_camera -c SG2_IMX390C_5300_GMSL2_96724_CPHY_x4 -m '0x0001 0x0000 0x0000 0x0000' -R -0 -1 -2 -s
```

3.3 SG5-IMX490C-5300-GMSL2-HXXX

```
# For Port1,link0
$ ./nvsipl_camera -c SG5_IMX490C_5300_GMSL2_96724_CPHY_x4 -m '0x0000 0x0000 0x0000 0x0001' -R -0 -1 -2 -s

# For Port2,link0
$ ./nvsipl_camera -c SG5_IMX490C_5300_GMSL2_CPHY_x4 -m '0x0000 0x0000 0x0001 0x0000' -R -0 -1 -2 -s

# For Port3,link0
$ ./nvsipl_camera -c SG5_IMX490C_5300_GMSL2_96724_CPHY_x4 -m '0x0000 0x0001 0x0000 0x0000' -R -0 -1 -2 -s

# For Port4,link0
$ ./nvsipl_camera -c SG5_IMX490C_5300_GMSL2_96724_CPHY_x4 -m '0x0001 0x0000 0x0000 0x0000' -R -0 -1 -2 -s
```

3.4 SG8S-AR0820C-5300-G2A-HXXX

```
# For Port1,link0
$ ./nvsipl_camera -c SG8S_AR0820C_5300_G2A_96724_CPHY_x4 -m '0x0000 0x0000 0x0000 0x0001' -R -0 -1 -2 -s

# For Port2,link0
$ ./nvsipl_camera -c SG8S_AR0820C_5300_G2A_CPHY_x4 -m '0x0000 0x0000 0x0001 0x0000' -R -0 -1 -2 -s

# For Port3,link0
$ ./nvsipl_camera -c SG8S_AR0820C_5300_G2A_96724_CPHY_x4 -m '0x0000 0x0001 0x0000 0x0000' -R -0 -1 -2 -s

# For Port4,link0
$ ./nvsipl_camera -c SG8S_AR0820C_5300_G2A_96724_CPHY_x4 -m '0x0001 0x0000 0x0000 0x0000' -R -0 -1 -2 -s
```

3.5 SG8-OX08DC-5300-_G2G-HXXX

```
# For Port1,link0
$ ./nvsipl_camera -c SG8_OX08DC_5300_G2G_96724_CPHY_x4 -m '0x0000 0x0000 0x0000 0x0001' -R -0 -1 -2 -s

# For Port2,link0
$ ./nvsipl_camera -c SG8_OX08DC_5300_G2G_CPHY_x4 -m '0x0000 0x0000 0x0001 0x0000' -R -0 -1 -2 -s

# For Port3,link0
$ ./nvsipl_camera -c SG8_OX08DC_5300_G2G_96724_CPHY_x4 -m '0x0000 0x0001 0x0000 0x0000' -R -0 -1 -2 -s

# For Port4,link0
$ ./nvsipl_camera -c SG8_OX08DC_5300_G2G_96724_CPHY_x4 -m '0x0001 0x0000 0x0000 0x0000' -R -0 -1 -2 -s
```

4.Show EEPROM data (Internal parameters)
```
$ ./nvsipl_camera -c SG2_AR0233C_5200_G2A_96724_CPHY_x4 -m '0x0000 0x0000 0x0000 0x0001' -R -0 -1 -2 -s -e
```

