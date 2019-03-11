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
        var time1_now_server,time1_now_client,time1_end,time1_server_client;
 
        time1_end=new Date("2019/02/11 19:25:0");//开始的时间
        time1_end=time1_end.getTime();//获取的是毫秒
 
        time1_now_server=new Date();//目前的时间
        time1_now_server=time1_now_server.getTime();//这里也是毫秒
        setTimeout("show_time()",1000);
 
        function show_time1()
        {
            var timer = document.getElementById("timer");
            var hourid = document.getElementById("hour");
            if(!timer){
                return ;
            }
            timer.innerHTML =time1_now_server;
 
            var time1_now,time1_distance,str1_time;
            var int_day1,int_hour1,int_minute1,int_second1;
            var time1_now=new Date();
            time1_now=time1_now.getTime();
            time1_distance=time1_now-time_end;
            if(time1_distance>0)
            {
                int_day1=Math.floor(time_distance1/86400000)
                time_distance1-=int_day1*86400000;
                int_hour1=Math.floor(time_distance1/3600000)
                time_distance1-=int_hour1*3600000;
                int_minute1=Math.floor(time_distance1/60000)
                time_distance1-=int_minute1*60000;
                int_second1=Math.floor(time_distance1/1000)
 
                if(int_hour1 < 10)
                    int_hour1="0"+int_hour1;
                if(int_minute1<10)
                    int_minute1="0"+int_minute1;
                if(int_second1<10)
                    int_second1="0"+int_second1;
                str_time="已经相恋<"+int_day1+"天"+int_hour1+"小时"+int_minute1+"分钟"+int_second1+"秒>";
                timer.innerHTML=str_time;
                setTimeout("show_time1()",1000);
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
<html>

	

