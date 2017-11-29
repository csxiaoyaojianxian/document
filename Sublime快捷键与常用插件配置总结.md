# Sublime快捷键与常用插件配置总结
## 1. 快捷键
ctrl + ~：打开控制台
Ctrl+Shift+P：打开命令面板
Ctrl+P：搜索项目中的文件
Ctrl+G：跳转到第几行
Ctrl+W：关闭当前打开文件
Ctrl+Shift+W：关闭所有打开文件
Ctrl+Shift+V：粘贴并格式化
Ctrl+D：选择单词，重复可增加选择下一个相同的单词
Ctrl+L：选择行，重复可依次增加选择下一行
Ctrl+Shift+L：选择多行
Ctrl+Shift+Enter：在当前行前插入新行
Ctrl+X：删除当前行
Ctrl+M：跳转到对应括号
Ctrl+U：软撤销，撤销光标位置
Ctrl+J：选择标签内容
Ctrl+F：查找内容
Ctrl+Shift+F：查找并替换
Ctrl+H：替换
Ctrl+R：前往 method
Ctrl+N：新建窗口
Ctrl+K+B：开关侧栏
Ctrl+Shift+M：选中当前括号内容，重复可选着括号本身
Ctrl+F2：设置/删除标记
Ctrl+/：注释当前行
Ctrl+Shift+/：当前位置插入注释
Ctrl+Alt+/：块注释，并Focus到首行，写注释说明用的
Ctrl+Shift+A：选择当前标签前后，修改标签用的
F11：全屏
Shift+F11：全屏免打扰模式，只编辑当前文件
Alt+F3：选择所有相同的词
Alt+.：闭合标签
Alt+Shift+数字：分屏显示
Alt+数字：切换打开第N个文件
Shift+右键拖动：光标多不，用来更改或插入列内容
鼠标的前进后退键可切换Tab文件
按Ctrl，依次点击或选取，可需要编辑的多个位置
按Ctrl+Shift+上下键，可替换行

Ctrl+D 选词 （反复按快捷键，即可继续向下同时选中下一个相同的文本进行同时编辑）
Ctrl+G 跳转到相应的行
Ctrl+J 合并行（已选择需要合并的多行时）
Ctrl+L 选择整行（按住-继续选择下行）
Ctrl+M 光标移动至括号内开始或结束的位置
Ctrl+T 词互换
Ctrl+U 软撤销
Ctrl+P 查找当前项目中的文件和快速搜索；输入 @ 查找文件主标题/函数；或者输入 : 跳转到文件某行；
Ctrl+R 快速列出/跳转到某个函数
Ctrl+K Backspace 从光标处删除至行首
Ctrl+K+B 开启/关闭侧边栏
Ctrl+KK 从光标处删除至行尾
Ctrl+K+T 折叠属性
Ctrl+K+U 改为大写
Ctrl+K+L 改为小写
Ctrl+K+0 展开所有
Ctrl+Enter 插入行后（快速换行）
Ctrl+Tab 当前窗口中的标签页切换
Ctrl+Shift+A 选择光标位置父标签对儿
Ctrl+Shift+D 复制光标所在整行，插入在该行之前
ctrl+shift+F 在文件夹内查找，与普通编辑器不同的地方是sublime允许添加多个文件夹进行查找
Ctrl+Shift+K 删除整行
Ctrl+Shift+L 鼠标选中多行（按下快捷键），即可同时编辑这些行
Ctrl+Shift+M 选择括号内的内容（按住-继续选择父括号）
Ctrl+Shift+P 打开命令面板
Ctrl+Shift+/ 注释已选择内容
Ctrl+Shift+↑可以移动此行代码，与上行互换
Ctrl+Shift+↓可以移动此行代码，与下行互换
Ctrl+Shift+[ 折叠代码
Ctrl+Shift+] 展开代码
Ctrl+Shift+Enter 光标前插入行
Ctrl+PageDown 、Ctrl+PageUp 文件按开启的前后顺序切换
Ctrl+Z 撤销
Ctrl+Y 恢复撤销
Ctrl+F2 设置/取消书签
Ctrl+/ 注释整行（如已选择内容，同“Ctrl+Shift+/”效果）
Ctrl+鼠标左键 可以同时选择要编辑的多处文本
Shift+鼠标右键（或使用鼠标中键）可以用鼠标进行竖向多行选择
Shift+F2 上一个书签
Shift+Tab 去除缩进
Alt+Shift+1（非小键盘）窗口分屏，恢复默认1屏
Alt+Shift+2 左右分屏-2列
Alt+Shift+3 左右分屏-3列
Alt+Shift+4 左右分屏-4列
Alt+Shift+5 等分4屏
Alt+Shift+8 垂直分屏-2屏
Alt+Shift+9 垂直分屏-3屏
Ctrl+Shift+分屏序号 将当前焦点页分配到分屏序号页
Alt+. 闭合当前标签
Alt+F3 选中文本按下快捷键，即可一次性选择全部的相同文本进行同时编辑
Tab 缩进 自动完成
F2 下一个书签
F6 检测语法错误
F9 行排序(按a-z)
F11 全屏模式

## 2. 安装Package Control
https://packagecontrol.io/installation
### 2.1 命令行安装：
按快捷键ctrl+~ 调出命名控制行，输入以下命令：
~~~
import urllib.request,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
~~~
### 2.2 手动安装
1. Preferences > Browse Packages
2. 从上层目录进入Installed Packages/目录
3. 将 Package Control.sublime-package 复制到Installed Packages/目录
4. 重启Sublime Text
## 3. 插件安装卸载
### 3.1 在线安装
快捷键 Ctrl+Shift+P（菜单 – Tools – Command Paletter），输入 install 选中Install Package并回车，搜索插件安装
### 3.2 离线安装
在github上下载插件解压，“Preferences”--->"Browse Packages"，打开包的位置，复制插件文件夹，重启
### 3.3 插件卸载
快捷键 ctrl+shift+p，输入remove package，选中删除
## 4. 常用插件
### 【emmet】
高效编写HTML和CSS
https://github.com/sergeche/emmet-sublime
**emmet 快捷键**
(1) 生成html5的结构代码
	! + tab
(2) 生成id名和类名
	标签名.类名#id名 + tab
	没有标签名.类名 + tab => div
(3) 生成子类标签
	标签名>子标签名>子标签名 + tab
(4) 带固定数量的标签:
	ul>li*5 + tab
(5) 带有序号名称	
	ul>li.abc$*3 + tab
(6) 生成带有内容的标签
	ul>li>a{data}*5 + tab
(7) css
	w30+tab => width:30px
	h30+tab => height:30px
	mg30+tab => margin:30px
	pd30+tab => padding:30px
	lh12px+tab => line-height:12px
	bg+tab => background

### 【SublimeLinter】
代码校验插件，支持 HTML、CSS、JS、PHP、Java、C++ 等16种语言
http://sublimelinter.com
**注意**：需要在sublime中额外安装相关lint并且全局安装node插件，才会有效
**相关lint**
> SublimeLinter-jshint
> SublimeLinter-jsxhint
> SublimeLinter-csslint
**全局安装node插件**
```shell
$ npm install -g jshint
$ npm install -g jsxhint
$ npm install -g csslint
```
### 【html-css-js prettify】
`ctrl + shift + h` 格式化代码
https://github.com/victorporof/Sublime-HTMLPrettify

### 【CSScomb】
CSS整理
http://csscomb.com/

### 【sublimeCodeintel】
`shift + ctrl + space` 代码自动提示
https://packagecontrol.io/packages/SublimeCodeIntel

### 【All Autocomplete】
搜索所有打开的文件来寻找匹配的提示词

### 【AutoFileName】
自动搜索提示相关的文件路径，如 js、css、img 等

### 【BracketHighlighter】
高亮选中的括号，支持代码折叠

### 【Color Highlighter】
色彩高亮

### 【FileHeader】
自动添加文件头
模板路径：`Data/Packages/FileHeader/template/`

### 【DocBlockr】
函数注释
https://github.com/spadgos/sublime-jsdocs

### 【Trimmer】
`ctrl + alt + s` 清除编写代码时由于错误或别的原因产生的一些不必要的空格
https://github.com/jonlabelle/Trimmer

### 【jQuery】
https://github.com/sublimetext/jquery

### 【SublimeServer】
启动本地服务器调试，在`tools`菜单中选择`start sublimeserver`

### 【gbk support】
中文支持，Sublime Text 本生不支持 gb2312，需要安装插件
https://github.com/chengsu/sublime-gbk-support

### 【ConvertToUTF8】
注意：需要修改 `Data/Packages/ConvertToUTF8/Default .sublime-keymap` 的快捷键设置，如 `ctrl+alt+shift+c`，避免与 colorPicker 冲突

### 【SideBarEnhancements】
侧栏右键功能增强
https://github.com/titoBouzout/SideBarEnhancements/tree/st3

### 【SublimeGit】
通过 `ctrl + shift + p` 使用git功能
```
git config --global user.name "username"
git config --global user.email "username@email.com"
```
http://sublimegit.readthedocs.io

### 【GitGutter】
高亮相对上次提交变动的行
修改配置
```
{
	"git_binary": "C:\\Program Files (x86)\\Git\\bin\\git.exe"
}
```
### 【AutoPrefixer】
`ctrl + shift + p` 输入调用进行CSS3私有前缀自动补全
https://github.com/sindresorhus/sublime-autoprefixer

### 【Terminal】
使用终端打开，支持使用快捷键
打开当前文件夹
`ctrl + shift + t` 
打开项目文件夹
`ctrl + alt + shift + t`
https://github.com/wbond/sublime_terminal

### 【ColorPicker】
`ctrl+shift+c` 调用取色器
http://weslly.github.io/ColorPicker

### 【Clipboard History】
`shift + ctrl + v` 剪切板历史记录
https://github.com/Jimbly/SublimeClipboardHistory

### 【CTags】
函数跳转

### 其他插件
【javascript & Nodejs Snippets】
快捷编码，可通过 `ctrl + shift + p` 输入snippets查看

【Can I Use】
兼容性检查
http://timkl.xyz/sublime-text-caniuse

【FileDiffs】
文件比较
https://github.com/colinta/SublimeFileDiffs

【Colorcoder】
高亮所有变量

【MarkdownEditing】
markdown编辑支持
`mdi + tab` 插入图片
`mdl + tab` 生成链接
https://github.com/mdesantis/MarkdownEditing

【OmniMarkupPreviewer】
预览markdown
Ctrl+Alt+O: Preview Markup in Browser.
Ctrl+Alt+X: Export Markup as HTML.
Ctrl+Alt+C: Copy Markup as HTML.
https://github.com/timonwong/OmniMarkupPreviewer

【PackageResourceViewer】
查看和编辑SublimeText附带的不同的包
https://github.com/skuroda/PackageResourceViewer

【soda-theme】
编码主题，Setting user里添加 "theme": "Soda Light 3.sublime-theme"
http://buymeasoda.github.io/soda-theme

Hex to HSL：自动转换颜色值
JsMinifier：自动压缩js文件
YUI Compressor：压缩JS和CSS文件
SFTP：直接编辑 FTP 或 SFTP 服务器上的文件
ftpsync：FTP ssh上传配置，安装成功配置host即可
ActualVim：使用vim

## 5. 其他
### 5.1 修改默认字体
修改`Settings - User`
```
"font_face": "微软雅黑",
"font_size": 14,
```
