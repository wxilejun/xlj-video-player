# XLJ Video Player (喜乐君 前端播放器)
### 详情了解
XLJ Video Player 简单的前端视频播放程序，**轻** `/` **快**
它是由 `html5` + `css3` + `javascript` 写出的
由XLJ(喜乐君)独立完成开发  
采用全前端模式，无需搭建PHP环境，上传网站根目录即可使用  
[预览](http://xlj0.com/dm/) **`/`** [博客](http://xlj0.com)  

注意，使用本程序前需要熟悉 `html` / `css` / `javascript`

### 文件结构
-css/ ***`存放CSS文件`***  
-js/ ***`存放JS文件`***  
-zy/ ***`播放器页面`***  
-index.html ***`首页`***

### 快速上手

#### 安装
直接下载本项目，上传到网站根目录解压，即可

#### 添加
添加视频，仅需要在/zy/html/ 新建一个html文件  
例如新建 `index_2_zy.html` 之后写入文件  
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>XLJ - zy</title>
    <link rel="stylesheet" href="../css/style.min.css">
    <link rel="stylesheet" href="../css/header.min.css">
    <link rel="stylesheet" href="../css/aliplayer-min.css">
    <script type="text/javascript" charset="utf-8" src="../js/player.js"></script>
</head>
<body>

  <script src="../js/alertdialog.js"></script>

        <header>
          <div class="toolbar">
              <span class="title">XLJ</span>
          </div>
        </header>
    
        <div id="player"></div>

        <div class="container margin_left_min margin_right_min margin_top_10">
          <span class="header_warning">由于XLJ的技术不够精湛所以完善的还不是很好，如果需要播放其他集数请先刷新页面再点击下面的按钮</span>
          <br>
          <span>XLJ是学生，因为时间和经济等原因，更新的时间不固定，如果发现有问题请先添加QQ群 <a href="https://shang.qq.com/wpa/qunwpa?idkey=f09cd58d91ec1d9def643e51f1365fb5008a4a07d4c07c6f7372123a794feebe">461909009</a></span>
          <br>
          <span>因为服务器带宽较大所以服务器费用都是XLJ独立支付的，如果你喜欢该剧，请前往&nbsp;<a href="https://xlj0.com">XLJ</a>&nbsp;赞赏一下吧！<br>你的支持是我的动力！</span>
        </div>

        <div class="h margin_left_min margin_right_min">

          <ul class="menuh">
              <li class="li" onclick="a_a();">1</li>
              <li class="li" onclick="a_b();">2</li>
              <li class="li" onclick="a_c();">3</li>
              <li class="li" onclick="a_d();">4</li>
          </ul>

        </div>

        <!-- JavaScript -->
        <script>
         function a_a() {
          var player_1_1 = new Aliplayer({
          "id": "player",
          "source": "https://dm-1259696352.cos.ap-chengdu.myqcloud.com/dm/BD/yuanzhikong/1_1/%5BXYCC-SumiSora%5D%5B%5BYosuga%20no%20Sora%5D%5BBDRIP%5D%5BVol.1%20KazuhaHen%5D%5B01%5D%5BGB%5D%5B720P%5D%5Bx264_AAC%5D.mp4",
          "autoplay": true,
          "isLive": false,
          "rePlay": false,
          "playsinline": true,
          "preload": true,
          "controlBarVisibility": "hover",
          "useH5Prism": true
        }, function (player) {
            player.stop();
          }
        );
        }

        function a_b(){
          var player_1_2 = new Aliplayer({
          "id": "player",
          "source": "https://dm-1259696352.cos.ap-chengdu.myqcloud.com/dm/BD/yuanzhikong/1_2/%5BXYCC-SumiSora%5D%5B%5BYosuga%20no%20Sora%5D%5BBDRIP%5D%5BVol.1%20KazuhaHen%5D%5B02%5D%5BGB%5D%5B720P%5D%5Bx264_AAC%5D.mp4",
          "autoplay": true,
          "isLive": false,
          "rePlay": false,
          "playsinline": true,
          "preload": true,
          "controlBarVisibility": "hover",
          "useH5Prism": true
        }, function (player) {
            // alert("XLJ - 动漫收藏:加载完成");
          }
        );
        }

        function a_c(){
          var player_1_3 = new Aliplayer({
          "id": "player",
          "source": "https://dm-1259696352.cos.ap-chengdu.myqcloud.com/dm/BD/yuanzhikong/1_3/%5BXYCC-SumiSora%5D%5B%5BYosuga%20no%20Sora%5D%5BBDRIP%5D%5BVol.1%20KazuhaHen%5D%5B03%5D%5BGB%5D%5B720P%5D%5Bx264_AAC%5D.mp4",
          "autoplay": true,
          "isLive": false,
          "rePlay": false,
          "playsinline": true,
          "preload": true,
          "controlBarVisibility": "hover",
          "useH5Prism": true
        }, function (player) {
            // alert("XLJ - 动漫收藏:加载完成");
          }
        );
        }

        function a_d(){
          var player_1_4 = new Aliplayer({
          "id": "player",
          "source": "https://dm-1259696352.cos.ap-chengdu.myqcloud.com/dm/BD/yuanzhikong/1_4/%5BXYCC-SumiSora%5D%5B%5BYosuga%20no%20Sora%5D%5BBDRIP%5D%5BVol.1%20KazuhaHen%5D%5B04%5D%5BGB%5D%5B720P%5D%5Bx264_AAC%5D.mp4",
          "autoplay": true,
          "isLive": false,
          "rePlay": false,
          "playsinline": true,
          "preload": true,
          "controlBarVisibility": "hover",
          "useH5Prism": true
        }, function (player) {
            // alert("XLJ - 动漫收藏:加载完成");
          }
        );
        }
        </script>

        <script type="text/javascript" color="255,0,0" pointColor="255,0,0" opacity='0.7' zIndex="-2" count="100" src="../.././js/dist/canvas-nest.js"></script>
        <script type="text/javascript" src="../.././js/dist/canvas-nest.umd.js"></script>

</body>
</html>
```

### 关于版权
XLJ Video Player 采用 MIT协议发布于 Github
