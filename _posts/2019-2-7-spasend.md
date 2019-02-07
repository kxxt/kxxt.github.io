---
layout: post
title: '国防知识竞赛考试快速完毕方法'
subtitle: '国防知识竞赛考试快速完毕方法'
date: 2019-02-07
categories: school
tags: school education
---
## 引子
有时候,我们会遇到类似的烦人调查问卷,但又不得不去填 .
这时候,我们万能的F12就要登场了...
虽然它不能帮助我们拿高分,但它可以帮我们省些时间(滑稽).
(本文针对不会F12的一般同学,请巨佬跳过)
## 1. 进入答题界面 , 点击 F12 键
看上去像这样...
![img](../../../assets/img/Snipaste_2018-09-24_18-04-31.png)
## 2. 找到"控制台"或"Console"并单击
![img](../../../assets/img/Snipaste_2018-09-24_18-05-43.png)  
下方有用来输入的地方.

![img](../../../assets/img/Snipaste_2018-09-24_18-05-28.png)
## 3. 复制以下代码并回车

> [注] 其中乱填的可以改成你想要的内容,但请保留原有的双引号 .

```js
function tiankong(id,sub,val)
{
    var obj=document.getElementsByName("aa_"+id+"_0")[sub];
    if(obj!=null&&obj!=undefined)
    obj.value=val;
}
function xuanze(id){
    var obj=document.getElementsByName("aa_"+id);
    if(obj!=null&&obj!=undefined){
        for(var i=0;i<=3;i++){
            if(obj[i]!=null&&obj[i]!=undefined)if(Math.floor(Math.random()*(3 + 1))%2==0)obj[i].click();
        }
    }
}
function tiankongx(id,sub,val)
{
    var obj=document.getElementsByName("aa_"+id+"_"+sub)[0];
    if(obj!=null&&obj!=undefined)
    obj.value=val;
}
for(var i=3001;i<=3080;i++){
    for(var j=0;j<=7;j++){
        tiankong(i,j,"乱填的");
    }
}
for(var i=3081;i<=3175;i++){
    xuanze(i); xuanze(i);xuanze(i);xuanze(i);
}
for(var i=3176;i<=3215;i++){
    xuanze(i); xuanze(i);xuanze(i);xuanze(i);
}
```
## 4. 稍后片刻 , 乱填完成
*注意一定要稍等片刻才能看到结果*
![img](../../../assets/img/Snipaste_2018-09-24_18-05-54.png)
![img](../../../assets/img/Snipaste_2018-09-24_18-13-59.png)
## 5. 然后提交即可
