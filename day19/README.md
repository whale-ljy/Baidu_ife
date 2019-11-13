DOM
===
<p>选择器</p>
<ol>
<li>getElementById()</li>
<li>getElementsByTagName(): 返回s</li>
<li>getElementsByName()</li>
<li>childNodes[0]===firstNode   lastNode</li>
<li>parentNode</li>
</ol>

<p>高级选择器</p>
<ol>
<li>querySelector("#secId"): 选择id=secId</li>
<li>querySelectorAll("div span"): 选择div中的span</li>
<li>querySelectorAll("div>span"): 选择div中的span</li>
</ol>

<p>创建表格</p>
var table=document.createElement("table");<br />
var tbody=document.createElement("tbody");<br />
table.appendChild(tbody);<br />
tbody.insertRow(0);<br />
tbody.rows[0].insertCell(0);<br />
tbody.rows[0].cells[0].appendChild(document.createTextNode("cell 1,1"));<br />
tbody.rows[0].insertCell(1);<br />
tbody.rows[0].cells[1].appendChild(document.createTxtxNode("cell 1,2"));<br />
tbody.insertRow(1);<br />
tbody.rows[1].insertCell(0);<br />
tbody.rows[1].cells[0].appendChild(document.createTextNode("cell 2,1"));<br />
tbody.rows[1].insertCell(1);<br />
tbody.rows[1].cells[1].appendChild(document.createTextNode("cell 2,2"));<br />
