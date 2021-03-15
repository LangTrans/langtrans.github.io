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

<div class="highlight" style="background: #f0f0f0"><pre style="line-height: 125%;"><span></span>p<span style="color: #4070a0">"Hello World"</span>
inc <span style="color: #666666">=</span> (x) =&gt; x<span style="color: #666666">+</span><span style="color: #40a070">1</span>
add(x,y)=&gt;x<span style="color: #666666">+</span>y
print(<span style="color: #666666">!</span>[inc =&gt; <span style="color: #40a070">1..6</span>])
print<span style="color: #666666">|</span>inc<span style="color: #666666">|</span>inc(<span style="color: #40a070">1</span>)
<span style="color: #007020; font-weight: bold">try</span> inc(<span style="color: #4070a0">"1"</span>) Exception print(<span style="color: #4070a0">"Error:"</span>,err)
test <span style="color: #666666">=</span><span style="color: #4070a0">"test"</span>
<span style="color: #666666">=</span>test.replace(<span style="color: #4070a0">"test"</span>,<span style="color: #4070a0">""</span>)
x <span style="color: #666666">=</span> True
print((x<span style="color: #666666">||</span>False)<span style="color: #666666">?</span><span style="color: #4070a0">"Done"</span><span style="color: #666666">:</span><span style="color: #4070a0">"Failed"</span>)
print(<span style="color: #4070a0">'x is not defined'</span>) <span style="color: #007020; font-weight: bold">if</span> <span style="color: #666666">!</span>x
</pre></div>

#### Orginal Syntax

<div class="highlight" style="background: #f0f0f0"><pre style="line-height: 125%;"><span></span><span style="color: #007020">print</span>(<span style="color: #4070a0">"Hello World"</span>)
inc <span style="color: #666666">=</span> <span style="color: #007020; font-weight: bold">lambda</span> x: x<span style="color: #666666">+</span><span style="color: #40a070">1</span>
add <span style="color: #666666">=</span> <span style="color: #007020; font-weight: bold">lambda</span> x,y:x<span style="color: #666666">+</span>y
<span style="color: #007020">print</span>(<span style="color: #007020">list</span>(<span style="color: #007020">map</span>(inc,<span style="color: #007020">range</span>(<span style="color: #40a070">1</span>,<span style="color: #40a070">6</span><span style="color: #666666">+</span><span style="color: #40a070">1</span>))))
<span style="color: #007020">print</span>(inc(inc(<span style="color: #40a070">1</span>)))
<span style="color: #007020; font-weight: bold">try</span>:
  inc(<span style="color: #4070a0">"1"</span>)
<span style="color: #007020; font-weight: bold">except</span> <span style="color: #007020">Exception</span> <span style="color: #007020; font-weight: bold">as</span> err:
  <span style="color: #007020">print</span>(<span style="color: #4070a0">"Error:"</span>,err)
test <span style="color: #666666">=</span><span style="color: #4070a0">"test"</span>
test<span style="color: #666666">=</span>test<span style="color: #666666">.</span>replace(<span style="color: #4070a0">"test"</span>,<span style="color: #4070a0">""</span>)
x <span style="color: #666666">=</span> <span style="color: #007020; font-weight: bold">True</span>
<span style="color: #007020">print</span>(<span style="color: #4070a0">"Done"</span> <span style="color: #007020; font-weight: bold">if</span> (x <span style="color: #007020; font-weight: bold">if</span> <span style="color: #4070a0">'x'</span> <span style="color: #007020; font-weight: bold">in</span> <span style="color: #007020">locals</span>() <span style="color: #007020; font-weight: bold">else</span> <span style="color: #007020; font-weight: bold">False</span>) <span style="color: #007020; font-weight: bold">else</span> <span style="color: #4070a0">"Failed"</span>)
<span style="color: #007020; font-weight: bold">if</span> <span style="color: #4070a0">'x'</span> <span style="color: #007020; font-weight: bold">not</span> <span style="color: #007020; font-weight: bold">in</span> <span style="color: #007020">locals</span>():
  <span style="color: #007020">print</span>(<span style="color: #4070a0">'x is not defined'</span>)
</pre></div>
Yaml files used here<br>
[New syntax](https://github.com/LangTrans/Py_Trans/blob/main/source.yaml)(For token extraction)<br>
[Template of LISP](https://github.com/LangTrans/Py_Trans/blob/main/target.yaml)
### LISP
#### Customized Syntax of LISP

<div class="highlight" style="background: #f0f0f0"><pre style="line-height: 125%;"><span></span>func printhis(s):
	<span style="color: #007020">format</span>(t,s)
printhis(<span style="color: #4070a0">"Customized!"</span>)
</pre></div>

#### Original Syntax 

<div class="highlight" style="background: #f0f0f0"><pre style="line-height: 125%;"><span></span>(defun printhis (s)
	(<span style="color: #007020">format</span> t s)
)
(printhis <span style="color: #4070a0">"Customized!"</span>)
</pre></div>
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
