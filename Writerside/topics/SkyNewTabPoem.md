# 云开诗词新标签页（旧版）
## 注意
* 本项目将停止维护，请前往云开诗词新标签页（新版）

## 简介
* 在新标签页随机展示不同的中国诗词，并提供日历、天气、倒数日、待办事项、专注模式、白噪音、快捷链接等实用功能
* 功能太多？也支持极简模式隐藏所有功能
* 支持语言：简体中文
* 所需权限：tabs、storage（专注模式）
* 日历来源：[https://www.mxnzp.com](https://www.mxnzp.com)
* 天气来源：[https://www.jinrishici.com](https://www.jinrishici.com)
* 噪音来源：[https://www.soundvery.com/](https://www.soundvery.com)
* 诗词来源：[https://www.jinrishici.com](https://www.jinrishici.com) 以及 [http://gushi.ci](http://gushi.ci)（诗词中的内容不代表作者任何观点）
* 开发支持：[JetBrains Open Source Support](https://jb.gg/OpenSourceSupport "跳转至 JetBrains Open Source Support")

## 主页
### 云开诗词新标签页（React + AntDesign）
* [GitHub 主页](https://github.com/xyk953651094/SkyNewTab-Poem-React "跳转至 GitHub 主页")
* [GitLab 主页](https://gitlab.com/xyk953651094/SkyNewTab-Poem-React "跳转至 GitLab 主页")
* 已上架至 Chrome、Edge、Firefox、~~Safari~~
### 云开诗词新标签页（Angular + NG Zorro）
* [GitHub 主页](https://github.com/xyk953651094/SkyNewTab-Poem-Angular "跳转至 GitHub 主页")
* [GitLab 主页](https://gitlab.com/xyk953651094/SkyNewTab-Poem-Angular "跳转至 GitLab 主页")
* 暂不上架

## 指南
### 诗词主题
* 新的诗词主题刷新后不会立即生效，必须等到下一个切换间隔才会生效
* 启用智能主题时不能使用诗词主题
* 禁用智能主题时才能使用诗词主题
* 诗词主题使用今日诗词 API V1（古诗词 · 一言 API），随机性更高
* 智能主题使用今日诗词 API V2，相关性更高
### 自定诗词
* 自定诗词可用于显示用户自行输入的文字
* 点击作者按钮即可使用自定诗词功能。若想关闭自定诗词，再次点击作者按钮，在弹出窗口中点击的“关闭自定诗词”按钮即可
* 诗词主题、智能主题、切换间隔等偏好设置在自定诗词下不会生效
### 字体
* 本插件并未内置任何字体，字体的显示效果与浏览器和系统有关
* 带衬线字体为：cursive 与 serif 类字体。无衬线字体为：sans-serif 类字体
* 通常系统自带的 cursive 与 serif 类字体不支持简繁切换，请自行安装相应支持简繁切换的字体
### 专注模式
* 开启专注模式后，访问黑名单中的网站将自动跳转至本插件
* 请先选择自动结束时间，再开启专注模式。专注模式开启后不支持修改自动结束时间，必需先关闭专注模式才能修改自动结束时间
* 播放白噪音时请不要随意关闭、刷新页面，否则白噪音会停止播放
* 若专注模式未成功拦截网站，尝试清空黑名单并重新添加，若无法解决问题，尝试菜单栏中的 “重置插件” 或者卸载后重新安装本插件
* 如果出现其它异常，请参考下方的异常处理
### Unsplash Access Key
* Unsplash Access Key 是使用 Unsplash API 获取图片的重要前提，但是存在流量限制
* 本插件使用的 Unsplash Access Key 由所有用户共享，因此当短时间内访问 Unsplash API 次数过多时会出现获取图片失败的情况
* 用户使用自己的 Unsplash Access Key 可以有效缓解以上问题
* 可参考《[使用 Shortcut 自动更换 Unsplash 的壁纸](https://ios.sspai.com/post/71295#!)》中的指南获取自己的 Unsplash Access Key
### 数据管理
* 请不要修改导出文件的内容
* 如果操作不当修改了导出文件的内容，请不要将其导入插件，否则可能导致数据丢失甚至插件异常
* 如果已经出现异常，请参考下方的异常处理
### 异常处理 ★★★
* 尝试 “重置设置” 按钮。注意 “重置设置” 将恢复初始设置，但会保留其他数据，例如倒数日和待办事项
* 若 “重置设置” 无法解决问题，尝试 “重置插件” 按钮。注意 “重置插件” 将清空插件所有数据并恢复初始状态
* 若 “重置插件” 无法解决问题，尝试关闭浏览器新标签页并清除浏览器缓存（有时可能需要多清理几次）
* 若清除浏览器缓存无法解决问题，尝试卸载后再重新安装本插件
* 若出现白屏，且卸载后再重新安装依然出现白屏，可能是 API 的问题，可尝试开启极简模式（关闭万年历 API 与天气 API），或者暂时禁用插件等待修复
* 最后，请参考[建议反馈](Report.md "前往建议反馈")将遇到的问题进行反馈，感谢您的支持

## 问题
### 为什么此插件需要 Storage、Tabs 权限？
答：专注模式需要 Tabs 权限阻止用户访问黑名单中的网站。同时也需要 Storage 权限存储用户添加的黑名单。此操作均在本地实现，请放心使用
### 为什么有的按钮点击后有反应，有的按钮点击后没反应？
答：当鼠标移至按钮上时，鼠标指针变为手指形状的按钮才可点击，鼠标指针没有变化的按钮无法点击
### 为什么清除浏览器缓存会重置插件？
答：本插件使用 LocalStorage 存储数据，清除浏览器缓存意味着清空插件的数据，请谨慎清除浏览器缓存
### 为什么日历信息不准确？
答：日历信息由第三方 API 提供，若出现不准确的情形，可点击日历弹窗右上角的更多信息按钮
### 为什么天气信息不准确？
答：天气信息由第三方 API 提供，若出现不准确的情形，可点击天气弹窗右上角的更多信息按钮
### 为什么刷新后还是显示上一次的诗词？
答：本插件设置了请求时间间隔，只有超过该时间间隔，才会请求并显示新的诗词
### 为什么打开智能主题后显示的诗词经常是《春江花月夜》？
答：这是今日诗词 API V2 的流量限制机制，请耐心等待或者关闭智能主题
### 为什么出现了 Unexpected end of JSON input 错误？
答：今日诗词 API 可能不支持海外访问，这是今日诗词 API 的问题，并不是本插件的问题，暂时无法修复
### 专注模式目前只有黑名单模式，以后会支持白名单模式吗？
答：经测试，白名单模式在不同的浏览器上会出现不同的问题（有些是浏览器本身的问题）。为了保证插件的稳定性，暂无发布白名单模式的计划
### 切换间隔为什么没有提供每次打开时立即切换的功能？
答：本插件使用的是今日诗词提供的免费 API，因此存在流量限制，高频率切换反而会导致插件使用体验下降
### 插件会发布 Safari 版吗？
答：目前已支持 Safari（iOS、iPadOS、MacOS），但苹果开发者账号费用较高，因此暂时没有发布 Safari 版的计划
### 插件会发布移动端吗？
答：目前已支持移动端（Android Firefox、iOS Safari、iPadOS Safari），但使用体验未达预期，因此暂时没有发布移动端的计划
### 除简体中文外，会支持其他语言吗？
答：暂时没有支持其他语言的计划