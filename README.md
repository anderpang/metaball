# metaball
metaball javascript计算


```javascript
//metaball数据
  var data=metaball(circle1, circle2, params.maxDistance);
  if(data){
      var cutDots=data.cutDots,
          ctrlDots=data.ctrlDots;
          
      ctx.beginPath();
        ctx.moveTo(cutDots[0].x,cutDots[0].y);
        ctx.bezierCurveTo(ctrlDots[0].x,ctrlDots[0].y,ctrlDots[3].x,ctrlDots[3].y,cutDots[3].x,cutDots[3].y);
        ctx.lineTo(cutDots[2].x,cutDots[2].y);
        ctx.bezierCurveTo(ctrlDots[2].x,ctrlDots[2].y,ctrlDots[1].x,ctrlDots[1].y,cutDots[1].x,cutDots[1].y);
      ctx.closePath(); 
      ctx.fill();     
  }
```  

![img](https://github.com/anderpang/metaball/blob/master/1.gif?raw=true)
  
  
