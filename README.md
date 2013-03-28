thooClock
=========

a jQuery analogue clock plugin with alarm function.

Implementation
--------------

<pre>
&lt;script language="javascript" type="text/javascript" src="http://code.jquery.com/jquery-latest.min.js"&gt;&lt;/script&gt; 
&lt;script language="javascript" type="text/javascript" src="js/jquery.thooClock.js"&gt;&lt;/script&gt;  	

&lt;script language="javascript" type="text/javascript"&gt;
  $('#myDIV').thooClock();
&lt;/script&gt;  
</pre>

Options
-------
<pre>
 $('#myDIV').thooClock({
    size:250,                               // size of the clock
    dialColor:'#000000',                    // foreground-color of dial can be defined as hex, colorstring, or rgb, rgba function
    dialBackgroundColor:'transparent',      // background-color of dial
    secondHandColor:'#F3A829',              // color of second hand
    minuteHandColor:'#222222',              // color of minute hand
    hourHandColor:'#222222',                // color of hour hand
    alarmHandColor:'#FFFFFF',               // color of alarm hand (alarm hand only visible if alarmTime is set to 'hh:mm')
    alarmHandTipColor:'#026729',            // color of tip of alarm hand
    hourCorrection:'+0',                    // hour correction e.g. +5 or -3
    alarmCount:1,                           // how many times should the onAlarm Callback function be fired
    alarmTime:'14:25',                      // alarm time hh:mm
    showNumerals:true,                      // show numerals on dial true/false
    brandText:'THOOYORK',                   // uppercase text on clock dial
    brandText2:'Germany',                   // lowercase text on clock dial
    onAlarm:function(){                     // alarm callback function 
      //callback on Alar
    },
    offAlarm:function(){                    // end alarm callback
      //callback on Alarm end
    },
    onEverySecond:function(){               // this function is fired on every second
      //callback do sttuff every second
    }
 });
</pre>

Set Alarm time from outside the plugin:
<pre>
  var strTime = '14:25'                       // must be hh:mm 
  $.fn.thooClock.changeTime(inp);
</pre>
