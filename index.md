# <center>韶翎裳 ♡ 桑小染</center>
    3479506443 ♡ 1060802477

<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>
<body>
    <div id="Layer1" style="position:fixed; left:0px; top:0px; width:100%; height:100%">  
    <img src="https://upload.cc/i1/2019/03/12/4R5CzG.jpg" width="100%" height="100%"/>  
</body>
</html>


#### <center><相恋于 2019年02月11日 19:55 星期一>

###### <center><2019ねん02がつ じゅういちにち 19:55 に恋する>     
<center>已经相恋</center>
<center>
<html>
<head>
    <style type="text/css">
        div{
            font-size:25px;
        }
    </style>
    <meta charset="utf-8">
    <meta http-equiv="Content-Type" content="text/html; charset=gb2312" />
    <title>相恋正时</title>
    <script type="text/javascript">
        var time_now_server,time_now_client,time_end,time_server_client;
 
        time_end=new Date("2019/02/11 19:25:0");//开始的时间
        time_end=time_end.getTime();//获取的是毫秒
 
        time_now_server=new Date();//目前的时间
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
                str_time="<"+int_day+"天"+int_hour+"小时"+int_minute+"分钟"+int_second+"秒>";
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
