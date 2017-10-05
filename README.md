# preload
图片预加载插件 -- jQuery插件
# 参数说明
## imgs：array or string
## options：object
ordered：如果设为true，图片按照顺序加载，即在加载完第一张图片后再加载第二张，默认为true；
eachOnLoad：在每张图片加载完成后的回调函数，如在显示图片加载进度时调用；
allOnLoad：所有图片加载完后的回调函数，隐藏进度条等等；
# 例子
## 1.有序加载
$.preload(imgs, {ordered: true});
## 2.无序加载
$.preload(imgs, {
    eachOnLoad: function() {},
    allOnLoad: function() {}
});
