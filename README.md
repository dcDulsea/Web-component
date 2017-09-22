# Web-component
Something i did
/*个人简历网站*/
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <!-- 上述3个meta标签*必须*放在最前面，任何其他内容都*必须*跟随其后！ -->
    <title>个人简历</title>

    <!-- Bootstrap -->
    <link href="css/resume.css" rel="stylesheet">

    <!-- HTML5 shim and Respond.js for IE8 support of HTML5 elements and media queries -->
    <!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
    <!--[if lt IE 9]>
    <script src="https://cdn.bootcss.com/html5shiv/3.7.3/html5shiv.min.js"></script>
    <script src="https://cdn.bootcss.com/respond.js/1.4.2/respond.min.js"></script>
    <![endif]-->
</head>
<body>
<header id="top" class="container-fluid">
    <!--导航条-->
    <nav id="myNav" class="navbar navbar-default">
        <div class="container-fluid">
            <!-- 我的logo -->
            <div id="myLogo" class="navbar-header">
                <a class="navbar-brand" href="#">周晨成(DC)</a>
            </div>
            <!-- 联系方式 -->
            <div id="myButton" class="navbar-right">
                <button type="button" class="btn btn-danger" data-toggle="modal" data-target=".smModal">
                    联系我(Contact me)
                </button>
                <div class="modal fade smModal" tabindex="-1">
                    <div class="modal-dialog modal-sm">
                        <div class="modal-content">
                            <div class="modal-header">
                                <button type="button" class="close" data-dismiss="modal"><span>&times;</span></button>
                                <h4 id="myTitle" class="modal-title">联系方式</h4>
                            </div>
                            <div class="modal-body">
                                <div class="media">
                                    <div class="media-left media-middle">
                                        <img class="media-object" src="img/photo.jpg">
                                    </div>
                                    <div id="myTitle" class="media-body">
                                        <p>所在地：上海</p>
                                        <p>手机：18621752302</p>
                                        <p>QQ：408867169</p>
                                        <p>Email：dc_sauce@163.com</p>
                                    </div>
                                </div>
                            </div>
                            <div class="modal-footer">
                                <button type="button" class="btn btn-default" data-dismiss="modal">关闭</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </nav>
    <!-- 关于我 -->
    <div id="aboutMe" class="row">
        <div class="col-xs-4 col-xs-offset-4">
            <h2 class="text-center">About Me</h2>
            <p class="text-center">
                一年左右的编码经验，熟练运用HTML/CSS（Less）/JavaScript前端三大语言。<br>熟悉并掌握Bootrstrap开源框架，编写移动设备优先的响应式网页，熟悉Less语言，能定制样式和手写Less语言。<br>了解Vue.js、React.js、Angular.js等主流框架。<br>个性温和，稳重和富有较强责任心，能快速融入一个新团队；<br>对编程非常感兴趣，能快速接收新的事物，与时俱进的学习新的框架结构技术；<br>具有良好的团队合作精神和协作能力，抗压能力强；<br>热爱钻研，擅长交流。
            </p>
        </div>
    </div>
</header>
<!-- 项目图片滚动播放 -->
<div class="container">
    <h2 class="text-center">项目截屏</h2>
    <div id="picCarousel" class="carousel slide" data-ride="carousel" data-interval="3000">
        <ol class="carousel-indicators">
            <li data-target="#picCarousel" data-slide-to="0" class="active"></li>
            <li data-target="#picCarousel" data-slide-to="1"></li>
        </ol>
        <div class="carousel-inner">
            <div class="item active">
                <img src="img/intel_1.png">
                <div class="carousel-caption">
                    <h3>Intel官网PC端</h3>
                </div>
            </div>
            <div class="item">
                <img src="img/intel_2.png">
                <div class="carousel-caption">
                    <h3>Intel官网PC端</h3>
                </div>
            </div>
        </div>
        <a href="#picCarousel" class="left carousel-control" data-slide="prev">
            <span class="glyphicon glyphicon-chevron-left"></span>
        </a>
        <a href="#picCarousel" class="right carousel-control" data-slide="next">
            <span class="glyphicon glyphicon-chevron-right"></span>
        </a>
    </div>
</div>
<!-- 详细介绍 -->
<div id="deTail" class="container">
   <ul class="nav nav-tabs nav-justified">
       <li class="active"><a href="#workExp" data-toggle="tab">工作经历</a></li>
       <li><a href="#eduExp" data-toggle="tab">教育背景</a></li>
       <li><a href="#studyExp" data-toggle="tab">培训经历</a></li>
       <li><a href="#itemExp" data-toggle="tab">项目经历</a></li>
   </ul>
    <div class="tab-content">
        <div class="tab-pane active" id="workExp">
            <p>时间：2017.03.20 至 2017.07.14</p>
            <p>公司：海牙湾国际贸易有限公司</p>
            <p>职位：客户执行</p>
            <p>工作内容：处理公司客户订单，与公司各部门配合协作完成客户采购销售订单。经手的客户有：美团点评、片仔癀、LVMH</p>
        </div>
        <div class="tab-pane" id="eduExp">
            <p>时间：2010.09 至 2014.07</p>
            <p>学校：福建工程学院</p>
            <p>专业：建筑环境与设备工程</p>
            <p>学历：本科 学士学位</p>
        </div>
        <div class="tab-pane" id="studyExp">
            <p>时间：2017.07 至今</p>
            <p>学校：上海达内信息科技有限公司</p>
            <p>专业：web前端开发工程师</p>
            <p>技能掌握：<br>1、擅长HTML5、CSS3语言，能够在项目中熟练结合使用CSS+DIV，手写出完整的静态页面并且能够解决跨浏览器的兼容问题。<br>2、熟悉JavaScript、DOM、等语言，js实现页面的动态交互和事件处理机制，熟悉了解ES5和ES6标准。<br>3、了解Bootstrap开源框架，可利用bootstrap全局CSS样式（栅格布局）、bootstrap组件、bootstrap对JS插件，编写移动设备优先的响应式网页，熟悉Less语言，能定制样式和手写Less语言。<br>4、熟练使用前端开发工具：Webstrom。</p>
        </div>
        <div class="tab-pane" id="itemExp">
            <h4>项目1</h4>
            <p>项目名称：响应式Intel官网模拟</p>
            <p>担任职责：前端开发</p>
            <p>项目说明：<br>以Intel官网为设计原型，模仿它的官网主页、登陆、注册等功能，主要负责内容：整个页面的HTML语言的编写，使用Bootstrap自定义网站所需样式，使用Less编译器进行CSS样式编译。根据不同终端编写不同的样式，例如有IPhone6、IPad和PC。</p>
            <p>项目链接：<a href="../intel/intel.html" target="_blank">Intel官网</a></p>
            <h4>项目2</h4>
            <p>项目名称：网页版2048小游戏模拟</p>
            <p>担任职责：前端开发</p>
            <p>项目说明：<br>以“2048”小游戏为设计原型，模仿他的游戏界面和游戏功能。项目分为两个阶段：第一阶段主要编写静态的HTML页面+css样式，第二阶段主要通过JavaScript添加用户响应，例如使用键盘的上下左右键来完成数字的移动与合并。</p>
            <p>项目链接：<a href="../2048/2048.html" target="_blank">2048</a></p>
        </div>
    </div>
</div>
<!-- 底部内容 -->
<footer class="container-fluid">
    <img src="img/dc.png" class="center-block">
    <h3 class="text-center">有意者请联系下方微信账号或扫面上方二维码或点击页头红色按钮</h3>
    <h4 class="text-center">微信个人账号：dclm920</h4>
</footer>
<!--*****************************************分割线*************************************************************-->
<!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
<script src="https://cdn.bootcss.com/jquery/1.12.4/jquery.min.js"></script>
<!-- Include all compiled plugins (below), or include individual files as needed -->
<script src="js/bootstrap.min.js"></script>
</html>
