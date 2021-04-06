## 
### some of c++11/c++14 features used in llvm

* final keyword : this keyword is used after class name so that we cannot inherit that class 
reference : https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/MacroArgs.h  
* explicit keyword :  
reference : https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/MacroInfo.h    
* auto keyword : if use auto keyword then there is no need to specify variable data type  
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/MacroInfo.h  
* nullptr : it is used to intialize pointer to null value  
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/HeaderSearch.h  
* move function : 
reference:  
* Templates :  //if we use templates then we can change datatypes without changing entire code//LLparser.h  
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/AST/APValue.h  
* delete keyword :         
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/HeaderSearch.h  
* non-static data members initialization :
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/HeaderSearch.h  
* default  keyword :
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/Pragma.h  
* range-based loops :
reference: https://github.com/llvm/llvm-project/blob/main/clang/lib/Frontend/CompilerInvocation.cpp  


### Class hierarchy
references:  
  https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Frontend/FrontendAction.h  
     https://github.com/llvm/llvm-project/blob/main/clang/include/clang/CodeGen/CodeGenAction.h
    
![tree](hello.png)

so much inheritance is used in llvm
                                                 
