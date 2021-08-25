# 自定义抽屉

> 图标请参考 https://www.mdui.org/docs/material_icon

!> 请遵循 JSON 语法，否则两行泪（哭

另外感谢 [MoLeft](http://www.moleft.cn/) 提供的 [快捷生成工具](http://cuckoo.moleft.cn/tool/drawer.php)

## 普通按钮

|name|value|remark|
|----|----|----|
|name|按钮名称||
|link|按钮链接|不需要可填“#”|
|icon|按钮图标|可前往 [MDUI Docs](https://www.mdui.org/docs/material_icon) 获取图标名|
|type|0||

### 举例

```json
{
  "name":"友人帐",
  "link":"https://xxx.xxx/links.html",
  "icon":"links",
  "type":"0"
}
```

## 归档按钮

|name|value|
|----|----|
|name|归档|
|link|#|
|icon|access_time|
|type|1|

### 举例

```json
{
  "name":"归档",
  "link":"#",
  "icon":"access_time",
  "type":"1"
}
```

## 分类按钮

|name|value|
|----|----|
|name|分类|
|link|#|
|icon|view_list|
|type|2|

### 举例

```json
{
  "name":"分类",
  "link":"#",
  "icon":"view_list",
  "type":"2"
}
```

## 页面按钮

|name|value|
|----|----|
|name|页面|
|link|#|
|icon|view_carousel|
|type|3|

### 举例

```json
{
  "name":"页面",
  "link":"#",
  "icon":"view_carousel",
  "type":"3"
}
```

## 列表按钮

|name|value|remark|
|----|----|----|
|name|按钮名称||
|link|按钮链接|不需要可填“#”|
|icon|按钮图标|可前往 [MDUI Docs](https://www.mdui.org/docs/material_icon) 获取图标名|
|type|4||
|list|子列表|注意遵循[ JSON 语法](http://www.w3school.com.cn/json/json_syntax.asp)|

### 举例

```json
{
  "name":"列表",
  "link":"#",
  "icon":"settings",
  "type":"4",
  "list": [{
  "name": "子列表",
  "link": "http://domain.com/"
  },{
    "name": "子列表",
    "link": "http://domain.com/"
  },{
    "name": "子列表",
    "link": "http://domain.com/"
  }]
}
```

## 分割线

|name|value|
|----|----|
|type|5|

```json
{
  "type":"5"
}
```

## Rss订阅按钮

|name|value|
|----|----|
|type|6|

- `"type"` 类型 6 为RSS订阅按钮。

```json
{
  "type":"6"
}
```

## 使用例

```json
[
  {
    "name":"分类",
    "link":"#",
    "icon":"view_list",
    "type":"2"
  },{
    "name":"归档",
    "link":"#",
    "icon":"access_time",
    "type":"1"
  },{
    "name":"页面",
    "link":"#",
    "icon":"view_carousel",
    "type":"3"
  },{
    "type":"5"
  },{
    "type":"6"
  }
]
```
