# vue-use-rxjs


1.先安装Rxjs   npm install rxjs --save

2.import {Subject} from "rxjs";
  const sendRowData$ = new Subject();
  export {
    sendRowData$,
    }
  可在全局可在单独文件，上述是在单独文件中。
  
3.sendRowData$.next({
                  data:n,
                }) 
  ----------------流传参
  
4.sendRowData$.subscribe((data)={
      ......相关操作，data是传过来的参数
})
