[LangTrans](https://github.com/LangTrans/LangTrans) is a developer tool to customize syntax of any programming language.

## Advantages
- You can customize any programming language with your needs.
- No need to create a new compiler/interpreter to use your preferred syntax.
- You can develop whole syntax or extend it with existing compiler/interpreter of any language.
- Code faster with your dialect for your domain.
- Knowledge about regular expression is the only prerequisite.
- Regular expression can be used with nesting support

## Example
### Python
#### Customized Syntax
```javascript
p"Hello World"
inc = (x) => x+1
add(x,y)=>x+y
print(![inc => 1..6])
print|inc|inc(1)
try inc("1") Exception print("Error:",err)
test ="test"
=test.replace("test","")
x = True
print((x||False)?"Done":"Failed")
print('x is not defined') if !x
```
#### Orginal Syntax
```python
print("Hello World")
inc = lambda x: x+1
add = lambda x,y:x+y
print(list(map(inc,range(1,6+1))))
print(inc(inc(1)))
try:
  inc("1")
except Exception as err:
  print("Error:",err)
test ="test"
test=test.replace("test","")
x = True
print("Done" if (x if 'x' in locals() else False) else "Failed")
if 'x' not in locals():
  print('x is not defined')
```
Yaml files used here<br>
[New syntax](https://github.com/LangTrans/Py_Trans/blob/main/source.yaml)(For token extraction)<br>
[Template of LISP](https://github.com/LangTrans/Py_Trans/blob/main/target.yaml)
### LISP
#### Customized Syntax of LISP

```python
func printhis(s):
	format(t,s)
printhis("Customized!")
```
#### Original Syntax 

```lisp
(defun printhis (s)
	(format t s)
)
(printhis "Customized!")
```
[New syntax](https://github.com/LangTrans/LangTrans/blob/main/example/source.yaml)<br>[Template of LISP](https://github.com/LangTrans/LangTrans/blob/main/example/target.yaml)

For more see the [Documentation](https://langtrans.readthedocs.io/en/latest/)

## Languages
* [Common Lisp](https://github.com/B-R-P/LISP_Trans)
* [Python](https://github.com/LangTrans/Py_Trans)
* [Lua](https://github.com/B-R-P/Lua_Trans)
* [Languages by community](https://langtrans.github.io/langtransrepos/)

[Share your language here](https://forms.gle/YDEKapaTZmJspyDeA)

## Download
- [Releases](https://github.com/LangTrans/LangTrans/releases)
- [Standalone](https://drive.google.com/uc?export=download&id=14lanbflcifeIM3PSCL3fF3rFxSBPrt7W)<br>
- [Installer](https://drive.google.com/uc?export=download&id=15soZJZCDrDP5KGVxvD5L9Sg7109XVc7y)

## Community
[<img src="https://discord.com/assets/2c21aeda16de354ba5334551a883b481.png" alt="Discord" style="height: 50px;width: 50px;"/>](https://discord.gg/3nDwppur5S)[<img src="https://avatars.githubusercontent.com/u/25838825?s=200&v=4" alt="Spectrum" style="height: 50px;width: 50px;"/>](https://spectrum.chat/langtrans-community)[<img src="https://www.gstatic.com/images/branding/product/2x/groups_48dp.png" alt="Google Groups" style="height: 50px;width: 50px;"/>](https://groups.google.com/g/langtrans-community)

LangTrans is licensed under [MIT License](https://raw.githubusercontent.com/B-R-P/LangTrans/main/LICENSE)
