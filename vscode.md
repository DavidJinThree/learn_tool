## download
**[download](https://code.visualstudio.com/docs/?dv=win)**

## config
**[史上最全vscode配置使用教程](https://zhuanlan.zhihu.com/p/113222681)**
### 设置中文
1. ctrl + shift + p
2. "configure language"
### 用户设置
> 文件>首选项>设置 
> 搜索workbench.settings.editor，选中json即可改成json设置


## 设置同步
> 首先要想在不同的设备间同步你的插件, 需要用到 Token 和Gist id
> Token 就是你把插件上传到 github 上时, 让你保存的那段字符，Gist id 在你上传插件的那台电脑上保存着
1. CTRL + SHIFT + P 我也不知道叫什么，暂且就叫它功能搜索功能吧
2. ALT + SHIFT + D 下载配置
3. ALT + SHIFT + U 上传配置

# vscode git


# 快捷键
## 行
- 重开一行: ctrl + enter; ctrl + shift + enter
- 删除一行: ctrl + x; ctrl + shift + k

## 词
- ctrl + d: 选中一个词

## 搜索
- ctrl + f: 搜索
- ctrl + alt + f: 替换
- ctrl + shift + f: 项目中搜索

- ctrl + \`: 打开终端
- ctrl + shift + [ : 折叠区域代码
- ctrl + shift + ] : 展开区域代码
- ctrl + / : 关闭行注释
- ctrl + alt + a : 块区域注释


# plugin
## vim
- [VSCode中使用Vim](https://zhuanlan.zhihu.com/p/141248420)
- [仓库](github.com/VSCodeVim/Vim)

### easymotion
- <leader> <leader> s <char> : 搜索

### surround
- d s <exsiting char>
- c s <exsiting char> <desired chat>

### sneak
- s<char><char>		; 下一个位置

### vscodevim tricks
- gd - jump to definition
- gh - 等价于鼠标悬停

## remote development




## vscode-icons
> 改变编辑器里面的文件图标

## Bracket Pair Colorizer
> 给嵌套的各种括号加上不同的颜色

## Auto Rename Tag
> 自动修改匹配的 HTML 标签

## Path Intellisense
> 智能路径提示

## Markdown Preview
> 实时预览 markdown

## Turbo Console Log
> 快捷添加 console.log，一键 注释 / 启用 / 删除 所有 console.log
### 快捷键
- ctrl + alt + l 选中变量之后，使用这个快捷键生成 console.log
- alt + shift + c 注释所有 console.log
- alt + shift + u 启用所有 console.log
- alt + shift + d 删除所有 console.log

## GitLens
> 详细的 Git 提交日志

## change-case
> 转换命名风格

## CSS Peek
> 定位 CSS 类名

## vscode-json
> 处理 JSON 文件

## Regex Previewer
> 实时预览正则表达式的效果