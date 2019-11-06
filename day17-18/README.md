js初步学习
===
学习课程：<a href="http://www.imooc.com/learn/10">慕课</a>
<ol>
<li>日期</li>
（1）今天日期var mydate=New Date();<br />
（2）mydate.getFullYear(); mydate.getMonth()+1; weekday[mydate.getDay()]; mydate.getHours();<br />
<li>Math</li>
（1）数值升序排序：sortNum(a,b) {return a-b //升序}<br />
mynum.Math.sort(sortNum);<br />
（2）mynum.Math.ceil();//往上取整 mynum.Math.floor();//往下取整<br />
（3）mynum.Math.random();<br />
<li>字符串<br /></li>
（1）大小写：myarr.toLowerCase(); myarr.toUpperCase();<br />
（2）返回指定字符位置：myarr.Math.indexOf("a",5);//从位置5开始search字符a<br />
（3）字符串分割：myarr.split(".",3);//以分割符.进行分割，至多分割3次<br />
（4）提取字符串：myarr.substring(3,5);//从位置3处提取5-3个字符 myarr.substr(3,5)//从位置3处提取5个字符<br />
（5）数组连接（显示为X，X）：var newarr=myarr1.concat(myarr2,myarr3);//合并数组1，2，3<br />
（6）以指定分割符连接（显示为X-X）：newarr.join("-");<br />
（7）颠倒数组：myarr.reverse();<br />
（8）插入字符：myarr.unshift("h");//前插入h myarr.push("h");//后插入h<br />
<li>计时器</li>
function startCount() {<br />
document.getElement("time").value=num;<br />
num++;<br />
setTimeout("startCount()",1000);<br />
}<br />
setTimeout("startCount()",1000);<br />
<li>返回/前进</li>
window.history.back(); window.history.forward();<br />


