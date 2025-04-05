# 欢迎进入类脑工作流发布帖子内反馈问题和下载细化模型等
## [点击加入类脑DC服务器](https://discord.gg/6kdVgVgcRx)
## [工作流帖子地址（需要进入服务器后答题才能看见）](https://discord.com/channels/1134557553011998840/1292880055193567263)

🌟 **ComfyUI 工作流功能指南 | 持续更新中**
*欢迎反馈 BUG 或改进建议，共同优化工作流体验*
—————————————————————————————————————————————
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

✈️ **各分区快速跳转**
- 数字1键 -> 跳转到底模与提示词编辑区
- 数字2键 -> 跳转到底图选择区
- 数字3键 -> 跳转到图像对比区
- 数字4键 -> 跳转到组管理区
- 数字5键 -> 跳转到参数控制区
- 数字6键 -> 跳转到可选文生图附加功能区
- 数字7键 -> 跳转到可选独立功能区

📚 **丰富的注释和使用指南**
- 清晰的操作指引

🖼️ **多种放大流程**
- `通用放大` | `混合放大` | `SD脚本放大`

👤 **部位细化**
- 提升图像的细节表现

🎨 **局部重绘**
- `Krita 互联高级涂鸦重绘` | `通用局部重绘`

🪄 **一键像素化**
- 无需额外下载底模和Lora的即用像素化

🧑‍🤝‍🧑 **提示词分区**
- 分区隔离元素污染

⚡ **出图加速**
- `条件时间步范围` + `WaveSpeed`
- 建议使用加速效果最佳的采样器：**euler**和**dpm系列**

🎨 **图像颜色匹配**
- 确保色彩一致性

🗂️ **各分区快捷开关**
- 侧边栏 | 节点管理，方便分类操作

⚙️ **独立的集成参数控制区**
- 全局参数控制：全局放大模型 | 全局平铺控制网模型 | 负面条件加速开关 | 分块采样开关
- 底图参数控制：步数 | CFG | 采样器 | 调度器
- 混合放大参数控制：步数 | CFG | 采样器 | 调度器 | 放大倍数 | 降噪幅度 | 控制网开关 | 控制网强度权重 | 控制网结束时间 | 加速开关
- 通用放大参数控制：步数 | CFG | 采样器 | 调度器 | 放大倍数 | 降噪幅度 | 控制网开关 | 控制网强度权重 | 控制网结束时间 | 加速开关
- SD放大参数控制：步数 | CFG | 采样器 | 调度器 | 放大倍数 | 降噪幅度 | 加速开关
- 部位细化参数控制：步数 | CFG | 采样器 | 调度器  | 脸部、眼部、手部、脚部、乳首 细化开关 | 脸部、眼部、手部、脚部、乳首 细化检测模型选择 | 加速开关

🌈 **背景移除**
- 独立可选的透明背景功能
—————————————————————————————————————————————
### 💻 **配置要求**
⚠️ **最低配置**：**8G 显存**
- 支持分辨率：`832x1216底图 + 2.25倍高清放大`
- 低显存方案：降低底图分辨率或高修倍数
—————————————————————————————————————————————
# ❗ 使用须知
# 🛑 **使用工作流前你 【必须更新你的内核】 **，否则有可能看不见必须阅读的注释！
# 🛑 **工作流【最左侧的红色注释】内容为必读 ！！！！！！**看完了还不懂再来问题！
# 🛑 **Manager 缺失插件地址已内置在注释中**
# 🛑 打开工作流前先删除汉化包插件【AIGODLIKE-ComfyUI-Translation】
- 秋叶管理器自带这个插件，请务必 **【删除它】**
- 这个汉化包已被其作者**放弃**，**不兼容新**版内核，会导致我的所有自定义设置节点名称**被还原**，设置分区将变得不明所以！所以你**必须删除它**！
- 删除它后，请务必**重启ComfyUI**，然后** 重 新 下 载 **工作流并打开它，这样自定义节点名称就正常了

—————————————————————————————————————————————
##  💬 酒馆独立版v0.3（玩酒馆文生图脚本的下这个）
- （独立更新 配合从前佬的文生图脚本食用）
- 质量版需要主工作流使用须知里的细化模型，请务必下载
## 酒馆文生图设置里用API文件！！！原工作流只是拿来测试能不能运行！！！
—————————————————————————————————————————————

最近的更新：
```
# 主工作流 v8.5.7 更新（推荐更新）
## 上个版本的更新日志（很重要，推荐观看）：
https://discord.com/channels/1134557553011998840/1292880055193567263/1357576441235247134
## 这次应该没什么问题了（大概<:neuroPray:1108327370206744576> ）
## 更新日志：
- 现在Lora堆也可以被Lora隔离选项影响
- 修正了Lora隔离实际上没有生效的问题（被自己蠢哭了<:neuroCry:1110064189839523881> ）
```

<details>
<summary>主工作流 v8.5.5 更新</summary>
# 主工作流 v8.5.5 更新：
## 这个版本理论上稳定性比之前要更强上一点
## ⚠️此次更新后工作流将使用新版的weilin提示词插件，使用Manager搜索缺失插件即可
- 原因：旧版weilin与easyloader疑似有冲突，有时会导致鬼图，具体触发方式不明，但可以确定是这两个的问题
- 我的词库怎么办？看指南（包括词库迁移和新版插件功能标注）

  [**如何使用WeiLin提示词编辑插件-1**](https://discord.com/channels/1134557553011998840/1292880055193567263/1357572468835094601)

  [**如何使用WeiLin提示词编辑插件-2**](https://discord.com/channels/1134557553011998840/1292880055193567263/1357572491526275072)

## 以下是更新日志：
1、提示词编辑插件改为新版weilin，解决偶发的鬼图问题
2、底模加载使用空白的伪正面和伪负面
3、单独设置一个纯净的无Lora管线，实现更彻底的隔离策略
4、混合放大一阶段的Lora隔离现在是可选项了，你可以在参数控制台找到它，相关的说明也一并补充，这里复制一下：
Lora隔离选项会在开启时完全屏蔽Lora对混合放大第一阶段的影响，对稳定高压Lora堆效果显著。
但是，开启后第一阶段的放大效果将完全取决于底模和画师串。
所以如果开启这个开关，你的画风最好和底模能对的上。
优点也是显而易见的，开启后混合放大将更加稳定，不过画面受底模的影响也会更重，所以用一个对的上画风的好底模就更加重要了（广告位招租）。
（比如使用凌乱的复杂画风Lora堆加上画风简洁干净的底模的时候，如果开启这个开关，那么放大后画面就会被底模简化，不过第二阶段无论如何也会被Lora影响，画面效果会被拉回来一点）
</details>


<details>
<summary>主工作流 v8.5.4 正式版更新</summary>
# 主工作流 v8.5.4 正式版更新：
- 此次更新的目的是稳定混合放大在高压Lora环境下的表现
- ⚠️更新后可能需要安装新插件，使用Manager搜索缺失插件即可
- 这个版本的混合放大对Lora堆的权重崩坏也有一定的修正效果
## 以下是更新日志：
1、Skimmed CFG回归
2、混合放大思路变更：
- 第一阶段完全隔绝Lora的影响，并对其应用PAG注意力引导，迭代次数降低为2，最终降噪幅度改为0.2
- 第二阶段走正常管线，被Lora影响，并使用SEG注意力引导
- 第二阶段的调度器改为exponential，降噪幅度降低为0.2
3、其他放大和细化的调度器统一为kl_optimal
4、 放大和细化的步数统一为30
5、补充了部分注释，排版略微变更
</details>

<details>
<summary>主工作流v8.5.3小型更新</summary>
# 主工作流v8.5.3小型更新：
## 主要针对混合放大调整稳定性：
- 第一阶段降噪幅度从0.1过渡到目标值
- 移除噪声注入相关的部分（兼容性不太行，尤其是V预测模型使用噪声注入反而降低质量）
- 混合放大的调度器改为`kl_optimal`
## 注意：
- 如果使用Lora后混合放大不稳定，请自行降低第一阶段和第二阶段的降噪幅度，默认都是0.3，你可以改成0.2甚至0.1，视情况而定
- 如果降低降噪后仍然不稳定，请切换到通用放大或者SD放大，并继续调整对应放大的降噪幅度（混合放大在高压Lora环境下稳定性并不好）
</details>


<details>
<summary>主工作流 8.5.2小型更新</summary>
# 主工作流 8.5.2小型更新：
## 更新日志：
- 细化设置参数区现在可以为每个部位的细化单独设置降噪幅度
- 取消底图的加速（负面加速还是能吃到的），底图步数默认改为28
- 混合放大、通用放大、SD放大、部位细化的默认采样器调度器组合改为euler normal，步数统一为20步
- 混合放大的第一阶段将会采样两次，混合放大的降噪幅度统一为0.25，噪声注入强度改为0.5
- 放大、细化的加速参数调整
- 为局部重绘添加加速
- 部分注释修正
- 默认关闭细化分区
</details>


<details>
<summary>v8.5大更新</summary>
# v8.5大更新
## 重大更改：
- 工作流排版分区全面优化，操作更便捷，功能划分更合理
- 文生图的所有分区现在都可以独立设置`采样器` `调度器` `步数` `CFG`，为细化分区添加细化模型参数，将参数设置分区合并为一个大分区，各个阶段的参数设置一目了然，能控制的参数大幅增加
- WaveSpeed应用思路变更，底图现在会单独使用质量更好的加速参数，放大阶段采用较为激进的加速策略，整体速度相较上个版本大幅度提升
- 添加一个独立的背景移除功能分区
## 其他更改：
- Weilin插件改为旧版，新版BUG太多
- 图像对比优化，未开启的分区不会显示图像
- 为混合放大和加速放大补充Tile预处理器，默认关闭控制网
- 添加Label节点对工作流分区进行备注
- 超绝友好的萌新指引箭头调转90度，并且更换为`优雅`的Label节点
- 工作流默认的采样器和调度器参数变更
- 注释完善
- 快捷键变更
- 底图完成的通知变更
- 组管理部分拆分，现在每个组管理部分都有总开关
</details>

<details>
<summary>v8.4.1小型更新</summary>
## v8.4.1小型更新
- 将底图选择部分独立到提示词分区旁边，便于操作
-  添加一个独立的可以查看所有文生图图像对比的分区
- 为混合放大和通用放大补充参数：控制网结束时间
- 调整混合放大和通用放大的参数：混合放大的控制网强度和权重调整为`0.85`，第二阶段降噪幅度调整为`0.3`，通用放大的控制网参数与混合放大同步
- 补充了缺失的组管理注释
- 部分注释修改
- 书签调整
- 放弃AYS调度器（质量和正常调度器差太多了）、移除水印处理部分（感觉不如...Krita）
- 修复了脸部细化不生效的问题，眼部细化改为默认关闭
</details>

<details>
<summary>v8.3.2更新日志</summary>
## v8.4大更新
- 分块采样与平铺控制网模型调整为全局参数
- 混合放大逻辑重构：
  - 前半段迭代次数设为1，取消AYS调度器，步数增至35，移除降噪约束
  - 后半段新增平铺控制网应用
- 通用放大新增可选控制网应用
- 取消分块放大分区（其所有功能已经可以在新版的通用放大上实现）
- 分块采样改为全局设置开关
- Lora堆默认保持开启状态，取消额外开关需求
- 默认CN模型加载数量调整为1，预处理器更换为AUX AIO
======================================================================
- 控制台分区重构为独立参数组：
  - 全局参数控制
  - 混合放大参数控制（新增控制网参数和放大倍数参数）
  - 通用放大参数控制（新增控制网参数和放大倍数参数）
  - 部位细化参数控制
- 简化 混合/通用放大 可控参数复杂度
======================================================================
- 像素化分区新增图像选择器支持快速重试
- 为所有分区标题添加键盘快捷键提示
- 书签节点位置重新整理，新增0键快速跳转至可选分区
- 可选分区布局重构优化
- Weilin提示词编辑节点改为为新版本
- 局部重绘移除无用节点，取消其AYS调度器
======================================================================
- 全局放大模型恢复为4x Ultrasharp
- 细化检测 新增眼部/脚部/乳首 检测
- 所有细化检测模型更换
- 细化分区取消AYS调度器
- 新增独立提示词分区（可选功能）
======================================================================
- 变量名中文化
- 注释完善
- 可选分区增加快速跳转
</details>
<details>
<summary>v8.3.2更新日志</summary>
## v8.3.2小型更新（可选更新）：
1、添加一键图像像素化节点PixelOE（需要手动克隆插件到本地）
- [Github地址](https://github.com/KohakuBlueleaf/PixelOE)
2、完善必看注释，避免歧义，注释里的模型要求部分增加细化模型和地址
3、添加一个超酷的萌新友好箭头
</details>
<details>
<summary>v8.3更新日志</summary>
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
</details>
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

