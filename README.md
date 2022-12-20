<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>表白墙初代</title>
  <style>
	 
    body {
      margin:0px;
		background: #f4c4f3;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #fc67fa, #f4c4f3);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #fc67fa, #f4c4f3); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

		
    }
    *{
      margin: 0px;
      padding: 0px;
    }
    li {
      list-style: none;
      width: 500px;
      height: 300px;
      margin-top: 5px;
    background: #00c3ff;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #ffff1c, #00c3ff);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #ffff1c, #00c3ff); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

	  }
    textarea{
      width: 200px;
      height: 80px;
    } 
  </style>
</head>
<body>
	<div style="padding:20px;margin-top:0px;height:210px;">
<h1>表白墙</h1>

<h2>要制作表白的爱心网站的可以找我制作作者qq：2239860745</h2>
<p>想要在本网站表白某某或吐槽某某可以加作者QQ，作者会将你的留言上传在本网站，可以匿名哦</p>


</div>

	<textarea name="" id=""></textarea>
  <button>发布</button>
  <ul>
     
  </ul>
  <script>
    //获取元素
    var btn = document.querySelector('button');
    var text = document.querySelector('textarea');
    var ul = document.querySelector('ul');
    //注册时间
    btn.onclick = function(){
      if(text.value == ''){
        alert("您没有输入内容。")
        return false;
      }else{
        var li = document.createElement('li');
        li.innerHTML = text.value;
        //ul.appendChild(li);
        ul.insertBefore(li,ul.children[0])
      }
      text.value='';
       
    }
  </script>
</body>
</html>
