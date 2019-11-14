# Repository for testing jshell

```
jshell> b= n;
|  Error:
|  incompatible types: possible lossy conversion from int to byte
|  b= n;
|     ^

jshell> C= n;
|  Error:
|  cannot find symbol
|    symbol:   variable C
|  C= n;
|  ^
```
### After errors fixed
``` 
  6 : b= (byte)n;
  
  b ==> 68
  
  7 : c= (char)n;
  
  c ==> 'D'
```
