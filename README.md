# vip视频解析
## 部署方法  
将vip-player.html上传到http服务器上即可。  
## 使用方法：
1. ​页面内输入网址：  
打开vip-player.html，在中间输入框中输入视频播放页的地址，点击播放即可。如果不能播放请尝试切换线路。
2. 网址参数调用：  
如http://xxx.com/vip-player.html?url=https://v.qq.com/x/cover/h05z5bsjxw544er.html，“url=”后面为视频播放页面地址，如果视频地址中含有中文则必须经过encodeURI()函数编码。网址打开后会自动解析播放，如果不能播放请尝试切换线路。  
3. 书签代码调用（推荐）：  
将以下代码保存为书签（请将“http://xxx.com/vip-player.html”修改为实际的地址），在视频播放页面点击书签即可自动解析播放，如果不能播放请尝试切换线路。  
>javascript:var domA=document.createElement('a');domA.href='http://xxx.com/vip-player.html?url='+location;domA.target='_self';domA.innerText=' ';domA.style.display='none';document.body.appendChild(domA);domA.click();
