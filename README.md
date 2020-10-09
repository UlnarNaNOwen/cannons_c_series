# C系列火炮说明文档

## 目录
[TOC]

- 如果不耐烦看请跳到文末看结论
- SE默认本地蓝图位置 ```C:\Users\你的用户名\AppData\Roaming\SpaceEngineers\Blueprints\local``` 请将蓝图拷贝到此处, **使用winRAR解压时注意不能文件夹套娃**

## 更新日志

```
----------<2020.10.07>----------
[0] 翻新了一遍受维护的火炮, 修改了毫无可读性的编组
[1] 取消了控制器的冗余设计, 火炮性能提升
[2] 新增了 C06 的复刻版本 C36

----------<2020.09.30>----------
[0] 新增了全新结构的火炮CR06
[1] 停止维护老的火炮, 现在只有C30, C32, C34, CH06, CR06五门火炮接受维护

----------<2020.08.16>----------
[0] 新增了 Cannon_C-C30 和 Cannon_C-C32, C26和C28有一定小瑕疵
[1] 新增了坦克 Tank-X10-C32

----------<2020.08.14>----------
更新说明: 新版本SE的转子和铰链抗拉伸能力降低, 导致火炮基座稳定性降低, 
因为后座抖动问题导致三联装的火炮故障率较高, 最好是别用
[0] 新增了全新结构的 Cannon_C-C26 和 Cannon_C-C28
[1] 修复了三联装基座工具栏部分项目失效的问题

----------<2020.08.13>----------
更新说明: 新版本SE的转子和铰链抗拉伸能力降低, 导致火炮基座稳定性降低, 
对高速火炮(C-C22, CH-06)的多联装略有影响, 正在尝试进行补偿(只能说K社智障)
[0] 略微降低了 Cannon_C-C22 核心部件的质量, 试图提升稳定性
[1] 新增了 CannonPedestal_CP-C10-M2 双联装基座
[2] 把群友 小渣渣 的鼠式坦克打包进来了, 可以用来测试火炮(雾)

----------<2020.08.12>----------
小更新
[0] 修复了三联装基座中有两个焊接器没有开启的问题
[1] 修复了 Cannon_C-C08 的基座工具栏项(摄像头查看)的错误
[2] 增加了 CannonPedestal_CP-C20 单联装基座
[3] 更新了新版本游戏中的炮弹速度在文档中的记录
[4] 修正了一些文档错误(错别字等)
[5] 说明文档(此文档)添加了一些内容

----------<2020.08.11>----------
系列全面重制
[0] 焊接器位置调整, 结构更加紧凑
[1] 调整了火炮整体结构, 降低了火炮高度(一格)
[2] 重制了附赠的火炮基座, 大幅降低火炮基座的体积
[3] 炮弹结构调整
[4] 全部火炮型号侧面装饰及按钮调整

----------<2020.08.01>----------
之前没写更新日志, 基本忘记更新了啥
[0] 新增火炮 Cannon_C-C24
```

## 火炮型号一览

|       型号        | 类型  |          说明          |    炮弹速度    |      适用环境       | 稳定性 |                                 备注                                 |
| :---------------: | :---: | :--------------------: | :------------: | :-----------------: | :----: | :------------------------------------------------------------------: |
| **Cannon_C-C06**  | 常规  |   中高速, 长管单轴炮   |     待测量     | 原生环境 & 高速环境 |   A    |                                 废弃                                 |
| **Cannon_C-C08**  | 常规  |  高速, 垂直长管双轴炮  |     待测量     | 原生环境 & 高速环境 |   A-   |                                 废弃                                 |
| **Cannon_C-C10**  | 常规  | 中低速, 垂直短管双轴炮 |     待测量     | 原生环境 & 高速环境 |   A    |                                 废弃                                 |
| **Cannon_C-C20**  | 破速  |  高速, 垂直长管双轴炮  |     待测量     | 原生环境 & 高速环境 |   D    |                                 废弃                                 |
| **Cannon_C-C22**  | 破速  |  高速, 垂直长管双轴炮  |     待测量     | 原生环境 & 高速环境 |   A-   |                                 废弃                                 |
| **Cannon_C-C24**  | 破速  | 中低速, 垂直短管双轴炮 |     待测量     | 原生环境 & 高速环境 |   A    |                                 废弃                                 |
| **Cannon_C-C26**  | 破速  |  高速, 水平长管三轴炮  |     待测量     | 原生环境 & 高速环境 |   B+   |                                 废弃                                 |
| **Cannon_C-C28**  | 破速  | 中低速, 水平短管双轴炮 |     待测量     | 原生环境 & 高速环境 |   A-   |                                 废弃                                 |
| **Cannon_C-C30**  | 破速  |  高速, 水平长管三轴炮  |  **约580m/s**  | 原生环境 & 高速环境 |   A-   |                          请使用改进型号 C36                          |
| **Cannon_C-C32**  | 破速  | 中低速, 水平短管双轴炮 |  **约270m/s**  | 原生环境 & 高速环境 |   A    |         目前唯一维护中的短管火炮, 有短管需求的话**推荐使用**         |
| **Cannon_C-C34**  | 破速  |  高速, 水平长管三轴炮  |  **约620m/s**  | 原生环境 & 高速环境 |   A    | **结构简约, 炮管轻巧, 后座更小, 性能良好, 稳定性卓越, 墙裂推荐使用** |
| **Cannon_C-C36**  | 破速  | 中高速, 水平长管单轴炮 |  **约340m/s**  | 原生环境 & 高速环境 |   B+   |      经典 C06 的破速重制版, 不过稳定性还是不太好, 不太推荐使用       |
| **Cannon_C-CH06** | 破速  |  特高速, 加长管五轴炮  |  **约750m/s**  | 原生环境 & 高速环境 |   C    |      炮管较长, 火炮较重, 量力而行(稳定性较差, 请使用新的CR系列)      |
| **Cannon_C-CR06** | 破速  |  特高速, 加长管四轴炮  |  **约800m/s**  | 原生环境 & 高速环境 |   B    |  炮管极长, 火炮极重, 量力而行(因作用力泄露问题不提供不含基座的版本)  |
|       -----       |       |                        |                |                     |        |                                                                      |
| **Cannon_C-C11**  | 测试  |     作用力平衡测试     | **400-500m/s** |  不适用于任何环境   |   F    |                             **请勿使用**                             |
| **Cannon_C-C12**  | 测试  |     作用力平衡测试     | **400-500m/s** |  不适用于任何环境   |   F    |                             **请勿使用**                             |
| **Cannon_C-C13**  | 测试  |     作用力平衡测试     | **400-500m/s** |  不适用于任何环境   |   F    |                             **请勿使用**                             |

## 火炮控制原件(定时器组)

- CannonControl_CC00: 标准火炮控住原件, 目前只有这一个, 最近添加了机枪保险功能 (现在不再会和机枪武器产生冲突)
  - 注: 所有的火炮都使用该型号控制原件
- CannonControl_CC-twin-G-R0: 可用于坦克的双联装火炮轮射|齐射控制原件 (可切换模式. 状态机控制器) (对定时器进行分组的版本) (定时器物理位置改变的版本)

## 火炮基座(附赠)

|           型号           |                                                    说明                                                     |
| :----------------------: | :---------------------------------------------------------------------------------------------------------: |
|  CannonPedestal_CP-C00   |                                  老式基座, 使用高级转子 (太过古老, 不维护)                                  |
|  CannonPedestal_CP-C10   |                              新式基座, 使用铰链, 出力更大 (太过古老, 不再维护)                              |
| CannonPedestal_CP-C10-M2 |                    CP-C10的二联装版本, 火炮横置, 装上火炮后外形科幻 (太过古老, 不再维护)                    |
| CannonPedestal_CP-C10-M3 |                                   CP-C10的三联装版本 (太过古老, 不再维护)                                   |
|  CannonPedestal_CP-C20   | 轻型基座, 火炮横置, 不过开炮后由于后座会导致轻微水平旋转, 通常情况下还是不要使用该基座 (太过古老, 不再维护) |
|  CannonPedestal_CP-C30   |                                    CP-10的前置版本 (太过古老, 不再维护)                                     |
|  CannonPedestal_CP-C40   |                                        CP-10的修改版本, **推荐使用**                                        |

## 载具(附赠)

|    型号    |                                说明                                 |                                         备注                                         |
| :--------: | :-----------------------------------------------------------------: | :----------------------------------------------------------------------------------: |
| Tank_T-X30 | 重型坦克, 装备双联装C34火炮, 搭载轮射状态机, 可一键切换轮射齐射模式 | **C系列官方指定车载火炮安装方式** (可供参考), 如果因安装问题导致火炮无法使用概不负责 |

## 火炮编组

|         编组名称          |        编组说明        |                                       备注                                        | 是否被定时器组影响 |           火炮开火过程中有何动作           |
| :-----------------------: | :--------------------: | :-------------------------------------------------------------------------------: | :----------------: | :----------------------------------------: |
|  **Decorations_cannon**   |         装饰品         |                                主要是显示器之类的                                 |         是         |     开炮时关闭编组, 装填完成后重新开启     |
|      **Guns_cannon**      |       加特林机枪       |                                   用于分离炮弹                                    |         是         | 先开启, 开炮中射击一次, 最后关闭(机枪保险) |
|     **Pistions_LIFT**     |       升降机活塞       |                                   便于拆装炮身                                    |         否         |                                            |
|    **Pistions_cannon**    |     火炮的蓄力活塞     | 活塞名称诸如 p0 p1 p2等等, p0是火炮最前端的(一个或多个)活塞, 编号越大距离前端越远 |         是         |       炮弹射出后伸展, 炮弹焊接后收缩       |
|   **Detachers_cannon**    |  炮管泄力转子(或铰链)  |                                 用来施放弹性势能                                  |         是         |         开炮时脱离, 活塞伸展后附着         |
|     **Rotors_FRONT**      |      火炮前部转子      |                  用于缓冲与抵消作用力泄露, 同时方便火炮调试改装                   |         否         |                                            |
|        **Turret**         | 用于脚本鼠标控制的编组 |                                                                                   |         -          |                                            |
|       **Hinges_V**        |   垂直旋转转子(铰链)   |                           基座上控制火炮垂直旋转的部件                            |         否         |                                            |
| **Warheads_cannon_shell** |       炮弹弹头组       |                                       炮弹                                        |         是         |          开炮后装备弹头(弹头保险)          |

## 火炮炮身右侧按钮功能(4个)

- 按钮主要用来拆卸, 调试, 修复火炮

| 位置(从右往左数) |         功能          |
| :--------------: | :-------------------: |
|        1         | 反转 Pistions_cannon  |
|        2         | Detachers_cannon 附着 |
|        3         | Detachers_cannon 脱离 |
|        4         |    开关红色瞄准线     |

## 基座合并块右侧按钮功能(2个)

| 位置  |                功能                |
| :---: | :--------------------------------: |
|  左   |   开关合并块, 用于拆卸和安装火炮   |
|  右   | 反转升降机活塞, 方便安装和拆卸火炮 |

## 重要提示
- Shell 开头的是炮弹蓝图(附送)
- **破速**: 在原版 100m/s 环境下打出火炮的额定速度(超过100m/s)
- 以上大部分火炮支持各种炮弹包括网格数较多的炮弹(可以堆叠较多弹头而不会导致炸膛, 比如**可以在炮弹上放座椅把工程师发射出去**, 不会导致炸膛)
- 火炮都是模块化接口设计的(用合并块连接), 可以很方便地在创造模式粘贴到基座上
- 你可以自己制造基座, **但我附赠了几个基座可以直接使用**. (我提供的基座未必能满足需求, 还请具体问题具体分析)
- **稳定性A及以上的火炮, 可以在高速移动下(100m/s)和按一定角速度旋转炮管时开火, 而不会轻易故障**, 稳定性A以下的火炮不保证走A和甩狙时的稳定性. CH和CR系列等重型火炮请于静止时开火. 
- **通常情况下小型载具无法搭载满配的 C34 火炮, 如果无法使用请根据载具吨位适当降低 C34 火炮的初速**. **降速方法**: 增加蓄力活塞的最小距离(**靠前的活塞的最小距离请保持大于等于靠后的活塞**), 可以参照 X30 坦克. (X30 上搭载的 C34 的具体设置: p0最小距离1.0m, p1最小距离0.5m, p2最小距离0.3m, p3最小距离0.0m. 该设置下初速约为420m/s)

## 结论
- 双数型号的炮是稳定版, 单数型号的炮不稳定, 用于测试和过渡, 请使用双数型号的火炮(现在包内不含单数型号的火炮)
- 推荐使用的炮型号是:  C30, C32, C34, CH06, CR06 不追求特别高的炮弹速度可以不用CH06和CR06, **以上所述版本中 C34 是当前最强大的火炮**
