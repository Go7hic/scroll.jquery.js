scroll.jquery.js
================

手机端滑动效果，适用于微信内活动推广的页面

主要功能：

####1.  share.js
微信分享功能，在微信中分享给好友或分享到自己的朋友圈时 设置图片，标题，描述。

在 index.html 里设置

```javascript
 $(function() {
            var shareTitle = 'PS 此乃何物';
            var imgUrl = '';//没有则取内容第一张图片，可以是隐藏元素
            var descContent = $("#div_fx_describe").text();
            wx_share_out(shareTitle,imgUrl,descContent);
        });
```
####2.  无限滚动
```
 var gd = true;//true:无限滚动，false:到最后页不能再滚
```
在 index.html 文件设置页面是否循环滚动

####3.  背景音乐

默认背景音乐是开启的, 自己更换背景音乐

```html
 <!-- 背景音乐 -->
        <div class="bg-music">
            <div class="music" id="musicWrap">
                <span class="close" onclick="musicPaused()">开关</span>
                <audio id="clickMusic" autoplay="autoplay" type="audio/mpeg">
                    <source src="music.mp3">
                    <source src="music.ogg">
                    <source src="music.wav">
                    你的浏览器不支持此功能
              </audio>
            </div>
        </div>
```
