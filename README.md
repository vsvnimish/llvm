## 
### some of c++11/c++14 features used in llvm

* final keyword : this keyword is used after class name so that we cannot inherit that class   
reference : https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/MacroArgs.h  
* explicit keyword :   
reference : https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/MacroInfo.h    
* auto keyword : if use auto keyword then there is no need to specify data type of variable    
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/MacroInfo.h  
* nullptr : it is used to intialize pointer to null value  
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/HeaderSearch.h  
* Templates : it is used for generic programming    
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/AST/APValue.h  
* delete keyword :             
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/HeaderSearch.h  
* intializer list : it is used to intialize all data members in class by default when we create an object to a class   
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/DirectoryLookup.h  
* default  keyword : in declaration of function if we intialize it to default then compiler will write some definition to that function   
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/Pragma.h  
* range-based loops : it is used to iterate over datastructure     
reference: https://github.com/llvm/llvm-project/blob/main/clang/lib/Frontend/CompilerInvocation.cpp
* using keyword :  it is used for entering into another class's scope  
reference: https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/MacroInfo.h  


### Class hierarchy
references:  
  https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Frontend/FrontendAction.h  
     https://github.com/llvm/llvm-project/blob/main/clang/include/clang/CodeGen/CodeGenAction.h
    
![tree](hello.png)

class hierarchy is tree which indicates parent-child relationship ,if class A inherits class B ,then class A is child of class B

### OOP design decisions for LLVM
 Abstraction : in this method we will place declartions and definitions of functions in seperate files ,so we will only give the file which contains declarations to the 
               user and we will not show or give the file which contains definition to the user , in llvm they maintained seperate files for declarations and definitions of                    functions   
 reference : https://github.com/llvm/llvm-project/blob/main/clang/include/clang/Lex/MacroArgs.h  
 
 Data hiding : 
 Inheritance :
 Modularity :
 Encapsulation :
 Polymorphism :
 
 

                                                 
