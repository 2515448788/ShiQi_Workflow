## 主要功能列表 📋
✨ **Promot-All-In-One 集成**
- 包含 WebUI 经典提示词编辑插件，自带 Lora 管理功能

🎨 **图像反推**
- 图像分析反推

🔗 **全局变量储存**
- 告别蜘蛛网般的复杂连接，简化管理
- 清晰明了的节点排版和分区规划

🌀 **集成式模型加载器 + ControlNet 堆 + Lora 堆**
- 高效管理与加载模型

📚 **丰富的注释和使用指南**
- 清晰的操作指引

🖼️ **多种放大流程**
- `通用放大` | `混合放大` | `分块放大` | `SD脚本放大`

👤 **自动脸部细化 + 自动手部细化**
- 提升图像的细节表现

🎨 **局部重绘**
- `Krita 互联高级涂鸦重绘` | `通用局部重绘`

⚡ **出图加速**
- `条件时间步范围` + `WaveSpeed` + `AYS 调度器`
- 建议使用加速效果最佳的采样器：**euler**和**dpmpp_2m**

🎨 **图像颜色匹配**
- 确保色彩一致性

🗂️ **各分区快捷开关**
- 侧边栏 | 节点管理，方便分类操作

⚙️ **集成式全局设置**
- `出图加速开关` 
- `全局CFG设置` 
- `全局采样器调度器设置` 
- `噪声注入开关` 
- `噪声注入强度控制`
- `迭代放大重绘幅度控制` 
- `TiledDiffusion开关` 
- `透明背景开关`

🌈 **LayerDiffusion 集成**
- 支持透明背景功能

🚫 **自动水印移除**
- 轻松去除图像水印
—————————————————————————————————————————————
### 💻 **配置要求**
⚠️ **最低配置**：**8G 显存**
- 支持分辨率：`832x1216底图 + 2.25倍高清放大`
- 低显存方案：降低底图分辨率或高修倍数
—————————————————————————————————————————————
## ❗ 使用须知
🛑 **使用工作流前你必须更新你的内核**，否则有可能看不见必须阅读的注释！
🛑 **工作流最左侧的红色注释内容为必读！！！！！！
🛑 **Manager 缺失插件地址已内置在注释中**



最近的更新：
```
## v8.3更新：
**1、控制台组节点拆分为：**
- 控制面板 通用
- 控制面板 混合放大
- 控制面板 其他
**2、控制面板新增参数控制：**
- 混合放大后半段降噪幅度
- 通用放大降噪幅度
**3、混合放大修改：**
- 移除PAG
- 前半段目标降噪幅度降低到`0.1`
- 噪声注入方式改为`CPU`
- 噪声注入目标强度降低到`0.1`
- 后半段降噪幅度降低到`0.2`
- ||修正后半段采样部分参数没有暴露的问题||
**4、细化分区的顺序改回旧版**
**5、细化分区改为默认关闭**
**6、部分注释位置调整、修正部分图片没有读取默认示例的问题**
## Tips：
- 此次旨在提高`控制台区域可操作性`和`混合放大的稳定性`
```
<details>
<summary>v8.2更新日志</summary>
## v8.2更新：
- 通用放大部分的放大模型统一
- 通用放大降噪幅度降低为`0.35`，步数增加到`35`
- 混合放大后半的通用放大降噪幅度降低为`0.35`、PAG强度降低到`1`，惩罚力度提升到`0.8`，图像迭代放大改为Latent迭代放大
- 主要设置部分节点整合为一个组节点（CUI这个组节点总算是好用了一会）
- 将混合放大后半段的通用放大也应用PAG的效果
- 全局随机种回归 ||这次没有忘记改回随机||
- 细化分区调整到高清放大之后（速度下降，但是细化效果应比之前好）
- 注释补充和修正
</details>
<details>
<summary>v8.1.1更新日志</summary>
8.1.1更新：
修正底图随机种被固定的问题
</details>
<details>
<summary>v8.1版本更新日志</summary>
v8.1小型更新：
1、修正开启加速导致Lora失效的问题
2、修正质量词错误
</details>
<details>
<summary>v8.0版本更新日志</summary>
## v8.0大更新：
1、工作流设置区域排版全面重构，新增大量变量储存节点，进一步规范工作流排版
2、组管理单独设置为一个分区
3、正面提示词新增一个后缀列表节点
4、主要设置部分新增设置项：
- 噪声注入强度 - 结束
- 迭代放大降噪幅度 - 起始
- 迭代放大降噪幅度 - 结束
5、新增一个显示完整正面提示词的节点
6、Lora堆最终应用位置调整
7、ControlNet堆应用位置调整，修复了之前ControlNet失效的问题，改为独立的可选分区（此分区只影响底图）
8、高清放大分区控制节点属性修改，最大选项只能为1
9、必看注释新增`Impact Subpack`插件需求
10、细化分区顺序调整，改为底图后，高清放大前
11、底图步数降低到`35`，AYS调度器相关采样步数降低到`15`
12、放大模型改为`RealESRGAN_2`（速度更快）
安装方法：`ComfyUI-Manager菜单内选择【Model Manager】,【Type】选择【upscale】，找到这个名称的模型点击安装，安装完毕后刷新即可`
13、注释补充与完善

⚠️ 注意：
- `质量词、采样器、调度器、CFG`需要根据模型要求自行修改，工作流里的默认参数并不适用于所有模型
- 默认的质量词`拼写有误`（少了个m），你可以自己加上或者换成自己常用的质量词
</details>
<details>
<summary>V7.8版本更新日志</summary>
V7.8版本更新：
1、必看注释节点改为适配markdown格式的版本，注释内容整理，优化观看体验，补充缺失插件的原址
2、提示词编辑部分补充一个固定正面提示词前缀列表的节点，你可以在这里填上你的质量词和画师串，这样就不用每次编辑提示词都重写了
3、WaveSpeed参数调整，默认参数改为官方推荐，但修改其max_consecutive _cache_list为1，使其每次使用缓存后都会使用一次原始采样，如此交替进行
4、保存图像节点改为was节点套件中的Image Save，图片将会跟保存日期分成文件夹保存
5、PAG的强度改为2，adaptive_scale改为0.5
6、所有使用AYS调度器的采样器步数略微增加到20
7、细化分区的检测改回yolo，细化采样节点改为easy use系列的细节修复节点
8、通用局部重绘的采样节点改为easy use的内部简易K采样器
9、注释整理与补充 节点和分区排版整理
</details>
<details>
<summary>v7.5版本更新日志</summary>
7.7.5版本更新：
1、PAG生效范围降低到0.3
2、面部手部细化分区更名为面部手部脚部细化，改为使用 segment anything 进行识别（第一次使用会在后台下载2个多G的模型，请务必开启TUN模式）
识别准确率更高，增加脚部的细化（有时候会识别成鞋子）
</details>
<details>
<summary>v7.4版本更新日志</summary>
7.7.4版本更新：
1、默认底图分辨率缩小，改回 832 x 1216 以适配更多模型
2、底图步数增加
3、wavespeed的加速生效区间改为0.35 ~ 1
4、负面条件生效范围改为0 ~ 0.7
5、迭代放大的PAG强度降低到3，生效区间增加到0.5，初始重绘幅度降低到0.3（希望可以缓解部分模型比目鱼的情况）
6、略微增大tile放大的重绘幅度
7、略微增大手部细化的重绘幅度
8、部分节点和分区排版整理，注释补充和修改
</details>

