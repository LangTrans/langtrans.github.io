[LangTrans](https://github.com/LangTrans/LangTrans) is a developer tool to customize syntax of any programming language.

## Benefits
- You can customize any programming language with your needs.
- No need to create a new compiler/interpreter to use your preferred syntax.
- You can develop whole syntax or extend it with existing compiler/interpreter of any language.
- Code faster with your dialect for your domain.
- Knowledge about regular expression is the only prerequisite.

## Example
### Python

```py
#Print
p"Hello World"
# Anonymous function
inc = (x) => x+1
# Lambda function
twice(x) = 2*x
# Single Line try-except
try inc("1") Exception print("Error:",err)
# Print Done if x is defined other wise Failed
print((x||True)?"Done":"Failed")
# Single Line if and check x defined or not
print('x is not defined') if !x
# Pipe Syntax
1 -> inc
|> print
# Reverse Pipe
print<-inc<-inc<-1
# Arithmetic operations with functions 
print((inc+twice)(3))
#Scope syntax work like in javascript
#scope1#
print("Scope1")
print("Done")

#scope2#
print("Scope2")
print("Done")

#PEP 359 - The "make" statement 
make type name(arg):
	x = 1
	if x == 1:
	    pass
	y = 3
make dict test: #Creating dictionary
    this =  "this"
    if this == "this":
        pass
    that = "that"
```

### LISP

```py
func printhis(s):
	format(t,s)
printhis("Customized!")
```

For more see the [Documentation](https://langtrans.readthedocs.io/en/latest/)

## Languages
* [Python](https://github.com/LangTrans/Py_Trans)
* [C](https://github.com/LangTrans/C_Trans)
* [Common Lisp](https://github.com/LangTrans/LISP_Trans)
* [Lua](https://github.com/LangTrans/Lua_Trans)
* [Languages by community](https://langtrans.github.io/langtransrepos/)

[Share your language here](https://forms.gle/YDEKapaTZmJspyDeA)

## Download
- [Releases](https://github.com/LangTrans/LangTrans/releases)
- [Standalone](https://github.com/LangTrans/LangTrans/releases/download/1.6/langtrans.exe)<br>
- [Installer](https://github.com/LangTrans/LangTrans/releases/download/1.6/LangTrans_Installer.exe)

## Community
[<img src="https://discord.com/assets/2c21aeda16de354ba5334551a883b481.png" alt="Discord" style="height: 70px;width: 70px;"/>](https://discord.gg/3nDwppur5S)[<img src="https://avatars.githubusercontent.com/u/25838825?s=200&v=4" alt="Spectrum" style="height: 70px;width: 70px;"/>](https://spectrum.chat/langtrans-community)[<img src="https://www.gstatic.com/images/branding/product/2x/groups_48dp.png" alt="Google Groups" style="height: 70px;width: 70px;"/>](https://groups.google.com/g/langtrans-community)

LangTrans is licensed under [MIT License](https://raw.githubusercontent.com/LangTrans/LangTrans/main/LICENSE)
