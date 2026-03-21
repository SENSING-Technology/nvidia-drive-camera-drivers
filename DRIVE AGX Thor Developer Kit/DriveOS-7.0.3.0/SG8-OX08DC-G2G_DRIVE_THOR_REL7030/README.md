
#### Jetpack version

* Drive OS: 7.0.3.0

#### Support camera list
* SG8-OX08DC-G2G-HXXX

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
$ sudo cp nito/* /usr/share/camera/
```

3.Show FPS

```
# For Port1,link0
$ ./nvsipl_camera -c SG8_OX08DC_G2G_96724_CPHY_x4 -m '0x0000 0x0000 0x0000 0x0001' -R -0 -1 -2 -s
$ ./nvsipl_camera -c SG8_OX08DC_G2G_96724_CPHY_x4 -m '0x0000 0x0000 0x0000 0x0001' -1 -2 -s

# For Port2,link0
$ ./nvsipl_camera -c SG8_OX08DC_G2G_CPHY_x4 -m '0x0000 0x0000 0x0001 0x0000' -R -0 -1 -2 -s
$ ./nvsipl_camera -c SG8_OX08DC_G2G_CPHY_x4 -m '0x0000 0x0000 0x0001 0x0000' -1 -2 -s

# For Port3,link0
$ ./nvsipl_camera -c SG8_OX08DC_G2G_96724_CPHY_x4 -m '0x0000 0x0001 0x0000 0x0000' -R -0 -1 -2 -s
$ ./nvsipl_camera -c SG8_OX08DC_G2G_96724_CPHY_x4 -m '0x0000 0x0001 0x0000 0x0000' -1 -2 -s

# For Port4,link0
$ ./nvsipl_camera -c SG8_OX08DC_G2G_96724_CPHY_x4 -m '0x0001 0x0000 0x0000 0x0000' -R -0 -1 -2 -s
$ ./nvsipl_camera -c SG8_OX08DC_G2G_96724_CPHY_x4 -m '0x0001 0x0000 0x0000 0x0000' -1 -2 -s
```

