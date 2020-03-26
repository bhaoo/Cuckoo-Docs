# 常见问题
<small>（这里收集了用户常出现的问题，会根据问题的提出进行更新）</small>

## 友链无法正常显示

友情链接需要“ [Links](https://github.com/bhaoo/Cuckoo/releases/download/1.0.2/Links.zip) ”插件支持哦，否则会导致出错。

## Aplayer 页面切换问题

请根据自己的需要填写以下内容至 **“控制台-外观-设置外观-功能-PJAX回调”** 中

### 停止播放

```json
if (typeof aplayers !== 'undefined'){
    for (var i = 0; i < aplayers.length; i++) {
        try {aplayers[i].destroy()} catch(e){}
    }
}
```

### 重载 Aplayer

```json
loadMeting();
```

## 如何获取文章CID

### 方法一

- 前往 **“管理-文章（或独立页面）-点击你想要获取ID的文章-进入编辑页面”**
- 查看地址栏 “https://xxx.xxx/admin/write-post.php?cid=123”
- 上方地址栏的 **123** 即为文章CID

### 方法二

- 前往 **“数据库-‘typecho_contents’表-通过查看文章名字从而找到其CID”**

