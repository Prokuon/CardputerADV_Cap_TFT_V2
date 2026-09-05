# Cap TFT V2 - 适用于 Cardputer ADV 的 2.8 寸屏幕扩展

Cap TFT V2 是为 Cardputer ADV 设计的屏幕扩展模块, 集成了一块 2.8 寸 ILI9341 屏幕 (320x240)

![](assets/20260829224411.jpg)

![](assets/20260829224434.jpg)

![](assets/20260829224449.jpg)

![](assets/20260829224501.jpg)

![](assets/20260829224518.jpg)

![](assets/20260829224551.jpg)

## BOM 清单

1. 3D 打印外壳 D1
2. 3D 打印外壳 D2
3. 3D 打印外壳 D3
4. 3D 打印外壳 L1
5. 3D 打印外壳 R1
6. 3D 打印外壳 S1
7. 3D 打印外壳 C1
8. 2.8 寸 ILI9341 屏幕
9. 内六角扁平头螺栓 M2x5 4 个
10. 内六角圆柱头螺栓 M2x5 3 个
11. 2.54mm 2x7P 双排直插针
12. 降压电源模块 (AMS1117-3.3V)

![](assets/20260829212842.jpg)

屏幕尺寸规格

![](assets/20260829213729.jpg)

降压电源模块参考图

![](assets/20260904195122.jpg)

## 组装说明

将降压电源模块粘贴到屏幕背面, 并按图示使用细导线连接屏幕与排针, 建议使用外径为 0.65mm 的线缆, 接线定义参考表格

![](assets/20260904195042.jpg)

屏幕

| GND  | VCC  | SCL  | SDA  | RES  | DC   | CS   | BLK  |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| 1    | 2    | 3    | 4    | 5    | 6    | 7    | 8    |

降压电源模块

| VIN  | VOUT |
| :--: | :--: |
| 10   | 2, 8 |
| GND  | GND  |
| 9    | 1    |

Cardputer

| G3   | G4   | G6   | G40  | G14  | G39  | G5   |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| 5    | x    | 6    | 3    | 4    | x    | 7    |
| 5VIN | GND  | 5VOUT| SDA  | SCL  | G13  | G15  |
| x    | 9    | 10   | x    | x    | x    | x    |

将屏幕安装至 D1

![](assets/20260829221756.jpg)

使用 4 个 M2x5 内六角扁平头螺栓将 D2 与 D3 安装至 D1

![](assets/20260829221645.jpg)

将排针安装至 S1

![](assets/20260829221531.jpg)

使用 1 个 M2x5 内六角圆柱头螺栓组装 C1 与 S1

![](assets/20260829221540.jpg)

将 L1 R1 安装至 D1

![](assets/20260829221547.jpg)

使用 2 个 M2x5 内六角圆柱头螺栓将 L1 R1 安装至 S1

![](assets/20260829221552.jpg)

组装完成

## Credits

- 新屏幕的选型参考了 tipflow 为 Cardputer ADV 设计的扩展屏幕, 项目地址: [M5 Cardputer Extended Screen](https://makerworld.com/zh/models/3054465-m5-cardputer-extended-screen?from=search#profileId-3436513)
- 屏幕扩展使用的固件基于 engneer-hamachan 的 [area512](https://github.com/engneer-hamachan/area512) 修改, 它是一个很棒的复古 OS, 风格类似美剧 Loki 中 TVA 组织使用的手持 Cyberdeck
