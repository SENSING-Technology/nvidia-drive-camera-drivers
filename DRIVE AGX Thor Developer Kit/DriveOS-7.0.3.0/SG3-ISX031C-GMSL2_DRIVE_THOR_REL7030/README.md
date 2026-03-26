#### DriveOS version

* DriveOS: 7.0.3.0

#### Supported camera list
* SG3-ISX031C-GMSL2-HXXX
* SG3-ISX031C-GMSL2F-HXXX

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

3.1 SG3-ISX031C-GMSL2-HXXX

```
# For Port1,link0
$ ./nvsipl_camera -c SG3_ISX031C_GMSL2_96724_CPHY_x4 -m '0x0000 0x0000 0x0000 0x0001' -R -0 -1 -2 -s

# For Port2,link0
$ ./nvsipl_camera -c SG3_ISX031C_GMSL2_CPHY_x4 -m '0x0000 0x0000 0x0001 0x0000' -R -0 -1 -2 -s

# For Port3,link0
$ ./nvsipl_camera -c SG3_ISX031C_GMSL2_96724_CPHY_x4 -m '0x0000 0x0001 0x0000 0x0000' -R -0 -1 -2 -s

# For Port4,link0
$ ./nvsipl_camera -c SG3_ISX031C_GMSL2_96724_CPHY_x4 -m '0x0001 0x0000 0x0000 0x0000' -R -0 -1 -2 -s
```

3.2 SG3-ISX031C-GMSL2F-HXXX

```
# For Port1,link0
$ ./nvsipl_camera -c SG3_ISX031C_GMSL2F_96724_CPHY_x4 -m '0x0000 0x0000 0x0000 0x0001' -R -0 -1 -2 -s

# For Port2,link0
$ ./nvsipl_camera -c SG3_ISX031C_GMSL2F_CPHY_x4 -m '0x0000 0x0000 0x0001 0x0000' -R -0 -1 -2 -s

# For Port3,link0
$ ./nvsipl_camera -c SG3_ISX031C_GMSL2F_96724_CPHY_x4 -m '0x0000 0x0001 0x0000 0x0000' -R -0 -1 -2 -s

# For Port4,link0
$ ./nvsipl_camera -c SG3_ISX031C_GMSL2F_96724_CPHY_x4 -m '0x0001 0x0000 0x0000 0x0000' -R -0 -1 -2 -s
```

4.Show Metadata (Exposure Time)
```
$ ./nvsipl_camera -c SG3_ISX031C_GMSL2_96724_CPHY_x4 -m '0x0000 0x0000 0x0000 0x0001' -R -0 -1 -2 -s -M
```

