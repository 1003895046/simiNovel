<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<meta name="viewport" content="width=device-width, initial-scale=1,maximum-scale=1, user-scalable=no">
		<meta name="apple-mobile-web-app-capable" content="yes">
        <meta name="apple-mobile-web-app-status-bar-style" content="black">
		<link rel="stylesheet" href="../../../assets/css/mui.min.css">
		<link rel="stylesheet" href="../../../assets/css/public.css">
		<style type="text/css">
			body{
				background: #fff;
			}
			.mui-grid-view.mui-grid-9{
				background: white;
				border: none
			}
			.mui-grid-view.mui-grid-9 .mui-table-view-cell{
				border: none
			}
			.mui-bar-nav~.mui-content{
				padding-top: 0
			}
			.mui-bar img{
				width: 24px;
				height: 24px	
			}
			*{touch-action: none;}
			.tab-item{
				    display: flex;
				    align-items: center;
				    flex-direction: column;
   					 justify-content: center;
   					 width: auto;
			}
			.mui-bar-tab{
				display: flex;
   				 justify-content: space-around;
			}
			.mui-active{
				color: #F72204
			}
		</style>
	</head>
	<body>
		<header class="mui-bar mui-bar-nav" style="color:;">
			　　　　<a href="#offCanvasSide" class="back mui-icon mui-action-menu  mui-pull-left  mui-icon-back"></a>
			　　　　<h1 id="title" class="mui-title" style="color:black;background-color:;">搜索</h1>
	　　</header>
		<div class="mui-content">
        
        <!-- MUI 搜索框 -->
        <div class="mui-input-row mui-search" id="searchForm">
            <input type="search" id="searchInput" onkeyup="enterSearch(event)" class="mui-input-clear" placeholder="请搜索小说或者作者">
        </div>
        
    </div>
  
    <nav class="mui-bar mui-bar-tab">
        <a class="tab-item mui-active" href="./home.html">
				<img src="../../../assets/img/Home_icon_001_01的副本.png">
				<span class="mui-tab-label">首页</span>
		</a>
        <a class="tab-item" href="./search.html">
				<img src="../../../assets/img/search_icon_001_011的副本.png">
				<span class="mui-tab-label">搜索</span>
		</a>
		<a class="tab-item" href="./Recharge.html">
				<img src="../../../assets/img/top_up_icon_001_01.png">
				<span class="mui-tab-label">充值</span>
		</a>
        <a class="tab-item" href="./mine.html">
				<img src="../../../assets/img/personal_center_icon_001_01
.png">
				<span class="mui-tab-label">我的</span>
		</a>
    </nav>
		<script src="../../../assets/js/public.js"></script>
		<script src="../../../assets/js/mui.min.js"></script>
		<script src="../../../assets/libs/jquery-3.2.1.min.js"></script>
		<script type="text/javascript">
			 mui.init({
          gestureConfig:{
           longtap: true //默认为false
          }
        });
        
        // 搜索事件,获取搜索关键词
        function enterSearch(event){
            if(event.keyCode == 13) {//用户点击回车的事件号为13
                var keyword = document.getElementById('searchInput').value;
                alert(keyword);
            }
        }
		</script>
	</body>
</html>
