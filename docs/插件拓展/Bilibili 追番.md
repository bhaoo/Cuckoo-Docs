!!! Warning

    请确保你的B站账号公开了追番列表

    请确保你的主机/服务器开启了cURL

## B站UID

填写自己的 UID 即可。

## 缓存时间

单位为“秒”，默认一天。

## 展示数量

默认为 10 个。

## 隐藏番剧

输入番剧 ID，多个 ID 用英文逗号隔开，就可以隐藏你所不想展示的番剧啦！

### 获取 番剧 ID

1. 前往缓存文件路径: `/usr/themes/Cuckoo/assets/cache/BilibiliFollow/BilibiliFollow.json`

    ```json hl_lines="5"
    [{
        "bangumi": [
        {
            "name": "\u5b64\u72ec\u6447\u6eda\uff01",
            "id": 28339735,
            "cover": {
            "large": "https:\/\/i0.hdslb.com\/bfs\/bangumi\/image\/d9d6284e0919ecfda41981c1f9119f993db62935.jpg",
            "square": "https:\/\/i0.hdslb.com\/bfs\/bangumi\/image\/cf3aab126a091b16e3f881c25303c22cd19c0127.png"
            },
            "url": "https:\/\/www.bilibili.com\/bangumi\/play\/ss43164",
            "type": "\u756a\u5267",
            "area": "\u65e5\u672c",
            "show": "\u516812\u8bdd",
            "evaluate": "\u7ef0\u53f7\u201c\u5c0f\u5b64\u72ec\u201d\u7684\u540e\u85e4\u72ec\uff0c\u662f\u4e00\u4e2a\u559c\u7231\u5409\u4ed6\u7684\u5b64\u72ec\u5c11\u5973\u3002\u7ecf\u5e38\u5728\u5bb6\u91cc\u72ec\u81ea\u5f39\u594f\u5409\u4ed6\uff0c\u4f46\u56e0\u4e3a\u4e00\u4e9b\u4e8b\u60c5\uff0c\u52a0\u5165\u4e86\u4f0a\u5730\u77e5\u8679\u590f\u9886\u8854\u7684\u201c\u7ebd\u5e26\u4e50\u961f\u201d\u3002\u4e0d\u6562\u5728\u4ed6\u4eba\u9762\u524d\u6f14\u594f\u7684\u540e\u85e4\uff0c\u80fd\u5426\u6210\u4e3a\u4e00\u4e2a\u51fa\u8272\u7684\u4e50\u961f\u6210\u5458\u5462\u2026\u2026...",
            "display": "1",
            "progress": ""
        },
        ...
    ],
    "time": 1700000000,
    "BilibiliUid": "xxxxxxxx",
    "amout": 10
    }]
    ```
   
2. 找到想要隐藏番剧所对应的对象，即可找到其 ID 力，如上述代码所示。

## Sessdate

如需获取观看进度需填写 Sessdata。

1. 打开 Bilibili。
2. 通过 ++f12++ 打开开发者工具。
3. 找到 `Application - Storage - Cookies - https://www.bilibili.com` 里面的 SESSDATA 复制进来即可。

!!! note

    无需担心账号被盗，数据均存在当前站点所在的数据库中，请妥善保管好自己的 SESSDATA。

## 更新缓存文件

删除缓存文件即可更新缓存文件

缓存文件路径: `/usr/themes/Cuckoo/assets/cache/BilibiliFollow/BilibiliFollow.json`

## 番剧列表空白
请检查上方的注意事项是否确保无误，或尝试更新缓存文件。

如果还是空白，请将番剧数量设置为30，并更新缓存文件。