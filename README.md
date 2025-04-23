# 原创 AV1 压制教程 HTML 网页版

本教程虽然相对于 x264、x265 教程严谨，并提供了测试数据提高严谨性，但仍仅具备业余参考价值。查阅本文要求读者已经明晰视频编码器的基本原理和一定细节。

为了减少网页加载和阅读难度，本教程超出概括叙述的内容都使用了折叠处理。

本教程提供了测试栏目，包括测试设计与实践。

## [点此打开](https://iavoe.github.io/av1-web-tutorial/HTML/index.html)

### 字体系统

本文使用了正文黑体，注解圆体和代码段字体共三套字体集。

- 正文黑体为首选[煮豆黑体 Zhudou Sans](https://github.com/Buernia/Zhudou-Sans)（中文）附件  
  - 辅以系统 Sans Serif（英文）
- 注解圆体为 Windows 的幼圆（中英文）附件
- 代码段的字体为传统代码段的 SFMono-Regular，Menlo，Monaco，Consolas（英文）  
辅以[狮尾圆体 Light](https://github.com/max32002/swei-gothic/blob/master)（中文）附件
- 公式段的字体为 [KaTeX Math Regular](https://github.com/KaTeX/katex-fonts/blob/master)（英文）附件（适配安卓）  
  - 辅以 Cochin，Georgia，Times，Times New Roman，serif

### 繁体中文支持

本教程由简体中文编写，可以通过安装浏览器插件来转换繁体及变体。效果不理想则请截图，并发送到本教程 Github 仓库中的 Issues，或 QQ 群里。

### 暗黑模式支持

本教程的所有图片在编写时已设为黑色背景。目前已验证 [Dark Reader](https://darkreader.org) 的显示效果可用。

### 打印机支持

打开教程后，在标题栏中可以将当前内容切换到打印排版。并切换回一般排版。转换效果不理想时请截图发送到本教程 Github 仓库中的 Issues，或 QQ 群里。

### English Support

This tutorial is proof-read with [TWP](https://addons.mozilla.org/en-US/firefox/addon/traduzir-paginas-web) webpage translation plugin (Google Translate API), and protects codes, pathes from being translated with HTML code tag. Despite some translation results in very long sentences, overall the sentences makes sense, and can be better with more large context ML translations.

#### English Support: Known issues

There are cases with the main clause in a sentence being enclosed in HTML code tag (which is ignored by translation plugin), resulting in bad context; In this case, manually copying the text to a translater would fix it:
- Source: ... 使用与 TM_PRED 类似的原理 ...
- Incorrect: ... Use with TM_PREDSimilar principles are used ...
- Correct: ... Uses similar principles as TM_PRED ...

There are verb-noun confustions in short words:
- Source: 应用预测
- Incorrect: Application Prediction
- Correct: Apply prediction

### 参考信息

见教程末尾。

### 打赏

<p align="center"><img src="bmc_qr.png"><br><img src="pp_tip_qr.png"></p>

——[Buy me a coffee 链接](https://buymeacoffee.com/iavoe)

——[PayPal 链接](https://www.paypal.com/qrcodes/managed/3e3e8b7f-27ed-4edc-a0fa-1b469e854a3c?utm_source=consapp)

<p align="center"><font size=1>——新纪录！这玩意现在年收入 0</font></p>

-----

当前版本（年，版，改）：2025.1.0<br>
联系方式：[Github：iAvoe]("https://github.com/iAvoe/iAvoe)，[QQ 群]("https://jq.qq.com/?_wv=1027&k=5YJFXyf")  
欢迎提交 pull-request 和 issues 指正
