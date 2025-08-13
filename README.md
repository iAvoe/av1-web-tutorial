# 原创 AV1 压制教程 HTML 网页版

本教程虽然相对于 x264、x265 教程严谨，并提供了测试数据提高严谨性，但仍仅具备业余参考价值。查阅本文要求读者已经明晰视频编码器的基本原理和一定细节。

## [点此打开](https://iavoe.github.io/av1-web-tutorial/HTML/index.html)

### 教程架构

- **概览**——视频编码的流程与 AV1 支持的新格式标准
- **编码**——AV1 标准下的算法与功能特点文图解析
- **参数**
  1. SVT-AV1 编码器
    1. 编码器（SVT-AV1）的实现说明
    2. 参数说明与推荐值
    3. 报错列表
- **附录**
  1. 画质指标科普
  2. 编码测试设计与跑分
  3. SVT-AV1(-PSY) 的下载与编译
    - 据普通用户群体的水平增加了更详细的引导
  4. 相关软件下载
  5. 参考文献说明

### 字体系统

本教程使用了正文黑体，注解圆体和代码段字体共三套字体集。

- 正文黑体为首选[煮豆黑体 Zhudou Sans](https://github.com/Buernia/Zhudou-Sans)（中文）附件  
  - 辅以系统 Sans Serif（英文）
- 注解圆体为 Windows 的幼圆（中英文）附件
- 代码段的字体为传统代码段的 SFMono-Regular，Menlo，Monaco，Consolas（英文）  
辅以[狮尾圆体 Light](https://github.com/max32002/swei-gothic/blob/master)（中文）附件
- 公式段的字体为 [KaTeX Math Regular](https://github.com/KaTeX/katex-fonts/blob/master)（英文）附件（适配安卓）  
  - 辅以 Cochin，Georgia，Times，Times New Roman，serif

本教程的代码块引入了 [higlight.js](https://highlightjs.org/#usage)（仅保留 cpp，PowerShell，Bash）和微调过的 docco.min.js。

### 移动端支持

本教程对移动端支持添加了以下功能：
1. 根据当前页面的宽度、高度调整内容大小
2. 点击图片轮训放大缩小
3. 使用兼容 Webkit/Blink 的独立字形（加粗、倾斜）字体文件

### 繁体中文支持

本教程由简体中文编写，可以通过安装浏览器插件来转换繁体及变体。效果不理想则请截图，并发送到本教程 Github 仓库中的 Issues，或 QQ 群里。

### 暗黑模式支持

本教程的所有图片在编写时已设为黑色背景。目前已验证 [Dark Reader](https://darkreader.org) 的显示效果可用。

### 打印与 PDF 生成支持

打开教程后，在标题栏中可以将当前内容在打印排版与一般排版间切换。转换效果不理想时请截图发送到本教程 Github 仓库中的 Issues，或 QQ 群里。

由于字数太多，所以建议只复制并打印需要的内容以促环保。

### English Support

This tutorial has been proof-read with [TWP](https://addons.mozilla.org/en-US/firefox/addon/traduzir-paginas-web) webpage translation plugin (Google Translate API), and protects codes, pathes from being translated with HTML code tag. Despite some translation results in very long sentences, overall the sentences makes sense, and can be better with more large context ML translations.

#### English Support: Known issues

There are cases with the main clause in a sentence being enclosed in HTML code tag (which is ignored by translation plugin), resulting in bad context; In this case, manually copying the text to a translater would fix it:
- Source: ... 使用与 TM_PRED 类似的原理 ...
- Incorrect: ... Use with TM_PREDSimilar principles are used ...
- Correct: ... Uses similar principles as TM_PRED ...

There are verb-noun confusions in short words:
- Source: 应用预测
- Incorrect: Application Prediction
- Correct: Apply prediction

### 参考信息

见教程末尾（不是 README/当前页末尾）。

### 后记

本教程是继 x264、x265 完整版教程的“续作”，其最明显的区别是配图数量翻倍、大量折叠处理的“概述之外”内容、引用性内容均辅以超链接指向出处、以及不同于以往的测试专用版块。

相比 x264、x265 教程，本教程提供了超过 90 张插图，并均匀分布到了 AV1 算法说明的版块中，以帮助读者更好地理解复杂的概念和技术细节。

由于信息量庞大，教程难免会有差错遗漏，追溯来源以确认信息可靠的需求就变得呼之欲出了。引用性内容的超链接对后期纠错查证，延伸阅读起到潜在的帮助，是属于“用时恨少”的细节。

新增的测试版块提供了对测试方法、涉及算法与软件、视频源的选择、测试命令与结果的内容。这些内容来自于实践，从而可以真正帮助到用户精确地了解参数值强度对编码的影响，而不再是造成思维二值化误解的“有些、较大、一定量”的形容词。

“欲穷千里目，更上一层楼”。总的来说，这些条件的达成使得本教程在可靠性、专业性和原创性方面有了显著提升，同时也极大地增强了用户体验。相比于纸上谈兵、空谈一番的 x264、x265 教程的存在价值更高。

### 打赏

<p align="center"><img src="bmc_qr.png"><br><img src="pp_tip_qr.png"></p>

——[Buy me a coffee 链接](https://buymeacoffee.com/iavoe)

——[PayPal 链接](https://www.paypal.com/qrcodes/managed/3e3e8b7f-27ed-4edc-a0fa-1b469e854a3c?utm_source=consapp)

<p align="center"><font size=1>——新纪录！这玩意现在年收入 0</font></p>

-----

当前版本（年，版，改）：2025.1.0<br>
联系方式：[Github Issues](https://github.com/iAvoe/av1-web-tutorial/issues)，[QQ 群](https://jq.qq.com/?_wv=1027&k=5YJFXyf)  
欢迎提交 pull-request 和 issues 指正