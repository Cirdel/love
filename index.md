# <center>韶翎裳 ♡ 桑小染</center>
##### <center>3479506443 - 1060802477</center>
#### <center><相恋于 2019年02月11日 19:55 星期一>
###### <center><2019ねん02がつ じゅういちにち 19:55 に恋する>

###### <center>-----==-----==-----==-----==-----==-----==-----==-----==-----==-----</center>

### <center>思念你的此时此刻是<center>
<center>
<html>
<head>
<meta charset="utf-8">
<title>js setInterVal()实时显示时间、日期</title>
<script>
window.onload = displayDate;	
function displayDate(){
	var date = new Date();
	var year = date.getFullYear();
	
	var month = date.getMonth()+1;
	month = ((month < 10)?"0":"") + month;
	var day = date.getDate();
	day = ((day < 10)?"0":"") + day;
	
	var hours = date.getHours();
	hours = ((hours < 10)?"0":"") + hours;
	
	var minutes  = date.getMinutes();
	minutes = ((minutes < 10)?"0":"") + minutes;
	
	var seconds = date.getSeconds();
	seconds = ((seconds<10)?"0":"") + seconds;
	
	var a = new Array("星期日にちようび","星期一げつようび","星期二かようび","星期三すいようび","星期四もくようび","星期五きんようび","星期六どようび");
	var day1 = date.getDay();
	day1 = a[day1];
	
	var currenttime = "<" + year + "年ねん" + month + "月がつ" + day + "日 " + hours + ":" + minutes + ":" + seconds + " " + day1 + ">";
	document.getElementById("demo").innerHTML = currenttime;
	
}
var  timer = window.setInterval(displayDate,1000);
function stopTimer(){
	window.clearInterval(timer);
}
</script>
</head>
<body>
 
<p id="demo"></p>

	
</body>
</html>
</center>
<center>
<html>
<head>
    <style type="text/css">
        div{
            font-size:10px;
        }
    </style>
    <meta charset="utf-8">
    <meta http-equiv="Content-Type" content="text/html; charset=gb2312" />
    <title>MARRY倒计时</title>
    <script type="text/javascript">
        var time_now_server,time_now_client,time_end,time_server_client;
 
        time_end=new Date("2026/08/11 00:00:0");//结束的时间
        time_end=time_end.getTime();//获取的是毫秒
 
        time_now_server=new Date();//开始的时间
        time_now_server=time_now_server.getTime();
        setTimeout("show_time()",1000);
 
        function show_time()
        {
            var timer = document.getElementById("timer");
            var hourid = document.getElementById("hour");
            if(!timer){
                return ;
            }
            timer.innerHTML =time_now_server;
 
            var time_now,time_distance,str_time;
            var int_day,int_hour,int_minute,int_second;
            var time_now=new Date();
            time_now=time_now.getTime();
            time_distance=time_end-time_now;
            if(time_distance>0)
            {
                int_day=Math.floor(time_distance/86400000)
                time_distance-=int_day*86400000;
                int_hour=Math.floor(time_distance/3600000)
                time_distance-=int_hour*3600000;
                int_minute=Math.floor(time_distance/60000)
                time_distance-=int_minute*60000;
                int_second=Math.floor(time_distance/1000)
 
                if(int_hour < 10)
                    int_hour="0"+int_hour;
                if(int_minute<10)
                    int_minute="0"+int_minute;
                if(int_second<10)
                    int_second="0"+int_second;
                str_time="离梦想の日还剩<"+int_day+"天"+int_hour+"小时"+int_minute+"分钟"+int_second+"秒>";
                timer.innerHTML=str_time;
                setTimeout("show_time()",1000);
            }
            else
            {
                timer.innerHTML =0;
            }
        }
    </script>
</head>
 
<body>
<div id="timer"></div>
</body>
</html>
<center>
<html>
<head>
    <style type="text/css">
        div{
            font-size:10px;
        }
    </style>
    <meta charset="utf-8">
    <meta http-equiv="Content-Type" content="text/html; charset=gb2312" />
    <title>MARRY倒计时</title>
    <script type="text/javascript">
        var time_now_server,time_now_client,time_end,time_server_client;
 
        time_end=new Date("2026/08/11 00:00:0");//结束的时间
        time_end=time_end.getTime();//获取的是毫秒
 
        time_now_server=new Date();//开始的时间
        time_now_server=time_now_server.getTime();
        setTimeout("show_time()",1000);
 
        function show_time()
        {
            var timer = document.getElementById("timer");
            var hourid = document.getElementById("hour");
            if(!timer){
                return ;
            }
            timer.innerHTML =time_now_server;
 
            var time_now,time_distance,str_time;
            var int_day,int_hour,int_minute,int_second;
            var time_now=new Date();
            time_now=time_now.getTime();
            time_distance=time_now-time_end;
            if(time_distance>0)
            {
                int_day=Math.floor(time_distance/86400000)
                time_distance-=int_day*86400000;
                int_hour=Math.floor(time_distance/3600000)
                time_distance-=int_hour*3600000;
                int_minute=Math.floor(time_distance/60000)
                time_distance-=int_minute*60000;
                int_second=Math.floor(time_distance/1000)
 
                if(int_hour < 10)
                    int_hour="0"+int_hour;
                if(int_minute<10)
                    int_minute="0"+int_minute;
                if(int_second<10)
                    int_second="0"+int_second;
                str_time="已经<"+int_day+"天"+int_hour+"小时"+int_minute+"分钟"+int_second+"秒>";
                timer.innerHTML=str_time;
                setTimeout("show_time()",1000);
            }
            else
            {
                timer.innerHTML =0;
            }
        }
    </script>
</head>
 
<body>
<div id="timer"></div>
</body>
</html>
