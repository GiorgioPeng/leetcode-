#思路：  
直接调用parseInt()函数读取整数，如果超过范围则进行一些相关操作  

```
var myAtoi = function(str) {
    var int = parseInt(str);
    var Max = Math.pow(2,31)-1;
    var Min = Math.pow(-2,31);
    if(int>Max)
        return Max;
    if(int<Min)
        return Min;
    if(isNaN(int))
        return 0;
    else return int;
    
};
```
