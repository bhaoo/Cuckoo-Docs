# PJAX回调

前往 **“设置外观-功能-PJAX回调”** 处填写即可。

## 百度统计

百度统计回调已内置在主题，无需再次填写

!> v1.0.4 存在BUG，因此需要自行添加回调内容，推荐升级版本

## 谷歌统计

```
if (typeof ga !== 'undefined'){
  ga('send', 'pageview', location.pathname + location.search);
};
```