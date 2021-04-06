## 
### some of c++11/c++14 features used in llvm
```
final keyword is used after class name so that we cannot inherit that class,and it is used in MacroArgs.h
reference : https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/MacroArgs.h
explicit keyword 
reference : https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/MacroInfo.h
auto - if use auto keyword then there is no need to specify variable data type
reference: 
nullptr - it is used to intialize pointer to null value
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/HeaderSearch.h
noexcept specifier
reference: 
Templates -  //if we use templates then we can change datatypes without changing entire code//LLparser.h
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/AST/APValue.h
//unique_ptr
//move function
delete keyword--        
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/HeaderSearch.h
non-static data members initialization 
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/HeaderSearch.h
default  keyword--    
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/Pragma.h
range-based loops  
reference: https://github.com/llvm/llvm-project/blob/main/clang/lib/Frontend/CompilerInvocation.cpp
```

### Class hierarchy
https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Frontend/FrontendAction.h

https://github.com/llvm/llvm-project/tree/main/clang/include/clang/CodeGen
 ![tree](hello.png)
                                                 
                                                 
### Example 3
```
       प्रारंभ():
           जबतक(क<5):       << Throws an initialisation error >>
                लिखो([क*क])
                क=क+1
```
### Example 4
```
          प्रारंभ():
              क=0
              क्ष=0
              जबतक(क=0):          << Throws conditional error in loop >>
        if(क्ष>क):
                         क्ष=क
                    क=क+1
```
### Example 5
```
    प्रारंभ():
            क=0
            जबतक(1):              << Infinite loop >>
                   क=क+1
```


## Examples which conforms our language specifications

### Example 1
```
प्रारंभ():
    इ =1
    जबतक( इ <= 10 ):        << Loop continues until इ becomes greaterthan or equal to 10 >>
      लिखो( [इ] )
      इ = इ + 1

```
### Example 2
```
प्रारंभ():
    पढ़े(ज)
    जबतक( ज <=20 ):         << Loop continues until ज becomes greaterthan or equal to 20 >>
        लिखो( [ज] )
        ज = ज + 2 

```
### Example 3
```
प्रारंभ():
    इ  = 1
    पढ़े( अ )   
    जबतक( इ<=10 ):        << Loop continues until इ becomes greaterthan or equal to 10 >>
        ब = अ * इ
        लिखो( [ब] )
        इ = इ + 1

```
### Example 4
```
प्रारंभ():
    व = 10
    य = 2
    जबतक( व+य ):                << Loop continues until व+य becomes 0 >>
        लिखो( [व] [य] )
         व = व - 1
         य = य - 1

```
### Example 5
```
प्रारंभ ():
    पढ़े( न )
    ण = न
    स = 0
    जबतक( न > 0 ):            << while loop continues till न becomes negative >>
        र = न % 10;
        स = स + र 
        न = न / 10;              
    लिखो( सम ऑफ़ डिजिट्स ऑफ़ [ण] इस [स] )   << Prints the sum of digits of न >>

```
