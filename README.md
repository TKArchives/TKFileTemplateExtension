# Toki的文件模板扩展(`File Template Extension`)

## 简述
本工程是提供给XCode使用的工程模板(`Project Template`).  
本工程内置安装脚本,默认安装在XCode包内(`/Applications/Xcode.app/Contents/Developer/Library/Xcode/Templates/Project Templates/Base/Other/TKFileTemplateExtension.xctemplate`).

本工程用于生成`文件模板扩展工程`, `文件模板扩展工程`用于`生成文件模板`.  
`生成文件模板`内置安装脚本,默认安装在XCode包内(`/Applications/Xcode.app/Contents/Developer/Library/Xcode/Templates/File Templates/模板分类/模板文件`)

## 文件向光参数介绍
### Information property
名字|类型|介绍
-|-|-
Kind|String|文件的类型（基本内容为标识码）
DefaultCompletionName|String|文件的默认名（多用于概括性描述文件类型）
SortOrder|String|排序优先级（实为数字）
Name|String|模版名字（会显示在创建文件时，选择文件类型的列表中，可以和*.xctemplate文件夹名字不同）
Description|String|详述
Summary|String|简述
Options|Array|创建文件页面的选项
### Option(Options 数组的条目)  
名字|类型|介绍
-|-|-
Required|Boolean|是否为必须填写的条目（选是则该条目必须填写，或有默认值）
Identifier|String|标识符（用于识别该选项的值）
Name|String|显示文案（显示在创建文件页面）
Description|String|条目详述（在创建文件页面,鼠标悬停在该条目操作区时，右侧显示该详述内容）
Type|String|条目类型（目前已知的有类型在下方例举）
NotPersisted|Boolean|是否不缓存条目的值（选否则该条目的值保留到下次创建同类型文件的时候）
### Type
名字|介绍
-|-
tent|文本
checkbox|复选框
popup|下拉表单（不可自由输入）
class|类名的下拉表单（可以自由输入）
