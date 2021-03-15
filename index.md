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

<div class="highlight" style="background: #263238"><pre style="line-height: 125%;"><span></span><span style="color: #EEFFFF">p</span><span style="color: #C3E88D">"Hello World"</span>
<span style="color: #EEFFFF">inc</span> <span style="color: #89DDFF">=</span> <span style="color: #89DDFF">(</span><span style="color: #EEFFFF">x</span><span style="color: #89DDFF">)</span> <span style="color: #89DDFF">=&gt;</span> <span style="color: #EEFFFF">x</span><span style="color: #89DDFF">+</span><span style="color: #F78C6C">1</span>
<span style="color: #EEFFFF">add</span><span style="color: #89DDFF">(</span><span style="color: #EEFFFF">x</span><span style="color: #89DDFF">,</span><span style="color: #EEFFFF">y</span><span style="color: #89DDFF">)=&gt;</span><span style="color: #EEFFFF">x</span><span style="color: #89DDFF">+</span><span style="color: #EEFFFF">y</span>
<span style="color: #EEFFFF">print</span><span style="color: #89DDFF">(![</span><span style="color: #EEFFFF">inc</span> <span style="color: #89DDFF">=&gt;</span> <span style="color: #F78C6C">1..6</span><span style="color: #89DDFF">])</span>
<span style="color: #EEFFFF">print</span><span style="color: #89DDFF">|</span><span style="color: #EEFFFF">inc</span><span style="color: #89DDFF">|</span><span style="color: #EEFFFF">inc</span><span style="color: #89DDFF">(</span><span style="color: #F78C6C">1</span><span style="color: #89DDFF">)</span>
<span style="color: #BB80B3">try</span> <span style="color: #EEFFFF">inc</span><span style="color: #89DDFF">(</span><span style="color: #C3E88D">"1"</span><span style="color: #89DDFF">)</span> <span style="color: #EEFFFF">Exception</span> <span style="color: #EEFFFF">print</span><span style="color: #89DDFF">(</span><span style="color: #C3E88D">"Error:"</span><span style="color: #89DDFF">,</span><span style="color: #EEFFFF">err</span><span style="color: #89DDFF">)</span>
<span style="color: #EEFFFF">test</span> <span style="color: #89DDFF">=</span><span style="color: #C3E88D">"test"</span>
<span style="color: #89DDFF">=</span><span style="color: #EEFFFF">test</span><span style="color: #89DDFF">.</span><span style="color: #EEFFFF">replace</span><span style="color: #89DDFF">(</span><span style="color: #C3E88D">"test"</span><span style="color: #89DDFF">,</span><span style="color: #C3E88D">""</span><span style="color: #89DDFF">)</span>
<span style="color: #EEFFFF">x</span> <span style="color: #89DDFF">=</span> <span style="color: #EEFFFF">True</span>
<span style="color: #EEFFFF">print</span><span style="color: #89DDFF">((</span><span style="color: #EEFFFF">x</span><span style="color: #89DDFF">||</span><span style="color: #EEFFFF">False</span><span style="color: #89DDFF">)?</span><span style="color: #C3E88D">"Done"</span><span style="color: #89DDFF">:</span><span style="color: #C3E88D">"Failed"</span><span style="color: #89DDFF">)</span>
<span style="color: #EEFFFF">print</span><span style="color: #89DDFF">(</span><span style="color: #C3E88D">'x is not defined'</span><span style="color: #89DDFF">)</span> <span style="color: #BB80B3">if</span> <span style="color: #89DDFF">!</span><span style="color: #EEFFFF">x</span>
</pre></div>

#### Orginal Syntax
<div class="highlight" style="background: #263238"><pre style="line-height: 125%;"><span></span><span style="color: #82AAFF">print</span><span style="color: #89DDFF">(</span><span style="color: #C3E88D">"Hello World"</span><span style="color: #89DDFF">)</span>
<span style="color: #EEFFFF">inc</span> <span style="color: #89DDFF">=</span> <span style="color: #BB80B3">lambda</span> <span style="color: #EEFFFF">x</span><span style="color: #89DDFF">:</span> <span style="color: #EEFFFF">x</span><span style="color: #89DDFF">+</span><span style="color: #F78C6C">1</span>
<span style="color: #EEFFFF">add</span> <span style="color: #89DDFF">=</span> <span style="color: #BB80B3">lambda</span> <span style="color: #EEFFFF">x</span><span style="color: #89DDFF">,</span><span style="color: #EEFFFF">y</span><span style="color: #89DDFF">:</span><span style="color: #EEFFFF">x</span><span style="color: #89DDFF">+</span><span style="color: #EEFFFF">y</span>
<span style="color: #82AAFF">print</span><span style="color: #89DDFF">(</span><span style="color: #82AAFF">list</span><span style="color: #89DDFF">(</span><span style="color: #82AAFF">map</span><span style="color: #89DDFF">(</span><span style="color: #EEFFFF">inc</span><span style="color: #89DDFF">,</span><span style="color: #82AAFF">range</span><span style="color: #89DDFF">(</span><span style="color: #F78C6C">1</span><span style="color: #89DDFF">,</span><span style="color: #F78C6C">6</span><span style="color: #89DDFF">+</span><span style="color: #F78C6C">1</span><span style="color: #89DDFF">))))</span>
<span style="color: #82AAFF">print</span><span style="color: #89DDFF">(</span><span style="color: #EEFFFF">inc</span><span style="color: #89DDFF">(</span><span style="color: #EEFFFF">inc</span><span style="color: #89DDFF">(</span><span style="color: #F78C6C">1</span><span style="color: #89DDFF">)))</span>
<span style="color: #BB80B3">try</span><span style="color: #89DDFF">:</span>
  <span style="color: #EEFFFF">inc</span><span style="color: #89DDFF">(</span><span style="color: #C3E88D">"1"</span><span style="color: #89DDFF">)</span>
<span style="color: #BB80B3">except</span> <span style="color: #FFCB6B">Exception</span> <span style="color: #BB80B3">as</span> <span style="color: #EEFFFF">err</span><span style="color: #89DDFF">:</span>
  <span style="color: #82AAFF">print</span><span style="color: #89DDFF">(</span><span style="color: #C3E88D">"Error:"</span><span style="color: #89DDFF">,</span><span style="color: #EEFFFF">err</span><span style="color: #89DDFF">)</span>
<span style="color: #EEFFFF">test</span> <span style="color: #89DDFF">=</span><span style="color: #C3E88D">"test"</span>
<span style="color: #EEFFFF">test</span><span style="color: #89DDFF">=</span><span style="color: #EEFFFF">test</span><span style="color: #89DDFF">.</span><span style="color: #EEFFFF">replace</span><span style="color: #89DDFF">(</span><span style="color: #C3E88D">"test"</span><span style="color: #89DDFF">,</span><span style="color: #C3E88D">""</span><span style="color: #89DDFF">)</span>
<span style="color: #EEFFFF">x</span> <span style="color: #89DDFF">=</span> <span style="color: #89DDFF">True</span>
<span style="color: #82AAFF">print</span><span style="color: #89DDFF">(</span><span style="color: #C3E88D">"Done"</span> <span style="color: #BB80B3">if</span> <span style="color: #89DDFF">(</span><span style="color: #EEFFFF">x</span> <span style="color: #BB80B3">if</span> <span style="color: #C3E88D">'x'</span> <span style="color: #89DDFF; font-style: italic">in</span> <span style="color: #82AAFF">locals</span><span style="color: #89DDFF">()</span> <span style="color: #BB80B3">else</span> <span style="color: #89DDFF">False)</span> <span style="color: #BB80B3">else</span> <span style="color: #C3E88D">"Failed"</span><span style="color: #89DDFF">)</span>
<span style="color: #BB80B3">if</span> <span style="color: #C3E88D">'x'</span> <span style="color: #89DDFF; font-style: italic">not</span> <span style="color: #89DDFF; font-style: italic">in</span> <span style="color: #82AAFF">locals</span><span style="color: #89DDFF">():</span>
  <span style="color: #82AAFF">print</span><span style="color: #89DDFF">(</span><span style="color: #C3E88D">'x is not defined'</span><span style="color: #89DDFF">)</span>
</pre></div>

Yaml files used here<br>
[New syntax](https://github.com/LangTrans/Py_Trans/blob/main/source.yaml)(For token extraction)<br>
[Template of LISP](https://github.com/LangTrans/Py_Trans/blob/main/target.yaml)
### LISP
#### Customized Syntax of LISP

<div class="highlight" style="background: #263238"><pre style="line-height: 125%;"><span></span><span style="color: #EEFFFF">func</span> <span style="color: #EEFFFF">printhis</span><span style="color: #89DDFF">(</span><span style="color: #EEFFFF">s</span><span style="color: #89DDFF">):</span>
	<span style="color: #82AAFF">format</span><span style="color: #89DDFF">(</span><span style="color: #EEFFFF">t</span><span style="color: #89DDFF">,</span><span style="color: #EEFFFF">s</span><span style="color: #89DDFF">)</span>
<span style="color: #EEFFFF">printhis</span><span style="color: #89DDFF">(</span><span style="color: #C3E88D">"Customized!"</span><span style="color: #89DDFF">)</span>
</pre></div>

#### Original Syntax 
<div class="highlight" style="background: #263238"><pre style="line-height: 125%;"><span></span><span style="color: #89DDFF">(</span><span style="color: #82AAFF">defun</span> <span style="color: #89DDFF">printhis</span> <span style="color: #89DDFF">(</span><span style="color: #82AAFF">s</span><span style="color: #89DDFF">)</span>
	<span style="color: #89DDFF">(</span><span style="color: #82AAFF">format</span> <span style="color: #89DDFF">t</span> <span style="color: #89DDFF">s)</span>
<span style="color: #89DDFF">)</span>
<span style="color: #89DDFF">(</span><span style="color: #82AAFF">printhis</span> <span style="color: #C3E88D">"Customized!"</span><span style="color: #89DDFF">)</span>
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
[<img src="https://discord.com/assets/2c21aeda16de354ba5334551a883b481.png" alt="Discord" style="height: 70px;width: 70px;"/>](https://discord.gg/3nDwppur5S)[<img src="https://avatars.githubusercontent.com/u/25838825?s=200&v=4" alt="Spectrum" style="height: 70px;width: 70px;"/>](https://spectrum.chat/langtrans-community)[<img src="https://www.gstatic.com/images/branding/product/2x/groups_48dp.png" alt="Google Groups" style="height: 70px;width: 70px;"/>](https://groups.google.com/g/langtrans-community)

LangTrans is licensed under [MIT License](https://raw.githubusercontent.com/B-R-P/LangTrans/main/LICENSE)
