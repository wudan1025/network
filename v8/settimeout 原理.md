<!--
 * @LastEditors: wudan01
 * @description: 文件描述
-->
> 另一个消息队列，维护了需要延迟执行的任务列表，包含了定时器和 chrome 内部需要延迟执行的任务
> 当创建定时器时，会将 回调放在这个队列中

> 时间存储 32bit , 时间最大值 2147483647, 超过会重置为0
```

function showName(){
  console.log("极客时间")
}
var timerID = setTimeout(showName,2147483648);//会被理解调用执行
```
