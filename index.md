[LangTrans](https://github.com/LangTrans/LangTrans) is a developer tool to customize syntax of any programming language.

### Advantages
- You can customize any programming language with your needs.
- No need to create a new compiler/interpreter to use your preferred syntax.
- You can create whole syntax or partially for an existing compiler/interpreter of any language.
- You can avoid repition of code and code faster.
* Knowledge about regular expression is all you need.

### Example
##### Customized Syntax of LISP

```python
func printhis(s):
	format(t,s)
printhis("Customized!")
```

##### Original Syntax 

```lisp
(defun printhis (s)
	(format t s)
)
(printhis "Customized!")
```
Yaml Files used here are [New syntax](https://github.com/LangTrans/LangTrans/blob/main/example/source.yaml)(Token extraction), [Template of LISP](https://github.com/LangTrans/LangTrans/blob/main/example/target.yaml)

For more see the [Documentation](https://langtrans.readthedocs.io/en/latest/)

### Languages
* [Lisp](https://github.com/LangTrans/LISP_Trans)
* [Lua](https://github.com/LangTrans/Lua_Trans)

### Community
[<img src="https://discord.com/assets/e05ead6e6ebc08df9291738d0aa6986d.png" alt="Discord" style="height: 100px;width: 100px;"/>](https://discord.gg/3nDwppur5S)

LangTrans is licensed under [MIT License](https://raw.githubusercontent.com/B-R-P/LangTrans/main/LICENSE)
