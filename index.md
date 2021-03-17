[LangTrans](https://github.com/LangTrans/LangTrans) is a developer tool to customize syntax of any programming language.

## Advantages
- You can customize any programming language with your needs.
- No need to create a new compiler/interpreter to use your preferred syntax.
- You can develop whole syntax or extend it with existing compiler/interpreter of any language.
- Code faster with your dialect for your domain.
- Knowledge about regular expression is the only prerequisite.

## Example
### Python
#### Customized Syntax

<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%;"><span></span><span style="color: #000000">p</span><span style="color: #4e9a06">"Hello World"</span>
<span style="color: #000000">inc</span> <span style="color: #ce5c00; font-weight: bold">=</span> <span style="color: #000000; font-weight: bold">(</span><span style="color: #000000">x</span><span style="color: #000000; font-weight: bold">)</span> <span style="color: #000000; font-weight: bold">=&gt;</span> <span style="color: #000000">x</span><span style="color: #ce5c00; font-weight: bold">+</span><span style="color: #0000cf; font-weight: bold">1</span>
<span style="color: #000000">add</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #000000">x</span><span style="color: #000000; font-weight: bold">,</span><span style="color: #000000">y</span><span style="color: #000000; font-weight: bold">)=&gt;</span><span style="color: #000000">x</span><span style="color: #ce5c00; font-weight: bold">+</span><span style="color: #000000">y</span>
<span style="color: #000000">print</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #ce5c00; font-weight: bold">!</span><span style="color: #000000; font-weight: bold">[</span><span style="color: #000000">inc</span> <span style="color: #000000; font-weight: bold">=&gt;</span> <span style="color: #0000cf; font-weight: bold">1..6</span><span style="color: #000000; font-weight: bold">])</span>
<span style="color: #000000">print</span><span style="color: #ce5c00; font-weight: bold">|</span><span style="color: #000000">inc</span><span style="color: #ce5c00; font-weight: bold">|</span><span style="color: #000000">inc</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #0000cf; font-weight: bold">1</span><span style="color: #000000; font-weight: bold">)</span>
<span style="color: #204a87; font-weight: bold">try</span> <span style="color: #000000">inc</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #4e9a06">"1"</span><span style="color: #000000; font-weight: bold">)</span> <span style="color: #000000">Exception</span> <span style="color: #000000">print</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #4e9a06">"Error:"</span><span style="color: #000000; font-weight: bold">,</span><span style="color: #000000">err</span><span style="color: #000000; font-weight: bold">)</span>
<span style="color: #000000">test</span> <span style="color: #ce5c00; font-weight: bold">=</span><span style="color: #4e9a06">"test"</span>
<span style="color: #ce5c00; font-weight: bold">=</span><span style="color: #000000">test</span><span style="color: #000000; font-weight: bold">.</span><span style="color: #000000">replace</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #4e9a06">"test"</span><span style="color: #000000; font-weight: bold">,</span><span style="color: #4e9a06">""</span><span style="color: #000000; font-weight: bold">)</span>
<span style="color: #000000">x</span> <span style="color: #ce5c00; font-weight: bold">=</span> <span style="color: #000000">True</span>
<span style="color: #000000">print</span><span style="color: #000000; font-weight: bold">((</span><span style="color: #000000">x</span><span style="color: #ce5c00; font-weight: bold">||</span><span style="color: #000000">False</span><span style="color: #000000; font-weight: bold">)</span><span style="color: #ce5c00; font-weight: bold">?</span><span style="color: #4e9a06">"Done"</span><span style="color: #ce5c00; font-weight: bold">:</span><span style="color: #4e9a06">"Failed"</span><span style="color: #000000; font-weight: bold">)</span>
<span style="color: #000000">print</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #4e9a06">'x is not defined'</span><span style="color: #000000; font-weight: bold">)</span> <span style="color: #204a87; font-weight: bold">if</span> <span style="color: #ce5c00; font-weight: bold">!</span><span style="color: #000000">x</span>
</pre></div>

#### Orginal Syntax
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%;"><span></span><span style="color: #204a87">print</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #4e9a06">"Hello World"</span><span style="color: #000000; font-weight: bold">)</span>
<span style="color: #000000">inc</span> <span style="color: #ce5c00; font-weight: bold">=</span> <span style="color: #204a87; font-weight: bold">lambda</span> <span style="color: #000000">x</span><span style="color: #000000; font-weight: bold">:</span> <span style="color: #000000">x</span><span style="color: #ce5c00; font-weight: bold">+</span><span style="color: #0000cf; font-weight: bold">1</span>
<span style="color: #000000">add</span> <span style="color: #ce5c00; font-weight: bold">=</span> <span style="color: #204a87; font-weight: bold">lambda</span> <span style="color: #000000">x</span><span style="color: #000000; font-weight: bold">,</span><span style="color: #000000">y</span><span style="color: #000000; font-weight: bold">:</span><span style="color: #000000">x</span><span style="color: #ce5c00; font-weight: bold">+</span><span style="color: #000000">y</span>
<span style="color: #204a87">print</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #204a87">list</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #204a87">map</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #000000">inc</span><span style="color: #000000; font-weight: bold">,</span><span style="color: #204a87">range</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #0000cf; font-weight: bold">1</span><span style="color: #000000; font-weight: bold">,</span><span style="color: #0000cf; font-weight: bold">6</span><span style="color: #ce5c00; font-weight: bold">+</span><span style="color: #0000cf; font-weight: bold">1</span><span style="color: #000000; font-weight: bold">))))</span>
<span style="color: #204a87">print</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #000000">inc</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #000000">inc</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #0000cf; font-weight: bold">1</span><span style="color: #000000; font-weight: bold">)))</span>
<span style="color: #204a87; font-weight: bold">try</span><span style="color: #000000; font-weight: bold">:</span>
  <span style="color: #000000">inc</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #4e9a06">"1"</span><span style="color: #000000; font-weight: bold">)</span>
<span style="color: #204a87; font-weight: bold">except</span> <span style="color: #cc0000; font-weight: bold">Exception</span> <span style="color: #204a87; font-weight: bold">as</span> <span style="color: #000000">err</span><span style="color: #000000; font-weight: bold">:</span>
  <span style="color: #204a87">print</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #4e9a06">"Error:"</span><span style="color: #000000; font-weight: bold">,</span><span style="color: #000000">err</span><span style="color: #000000; font-weight: bold">)</span>
<span style="color: #000000">test</span> <span style="color: #ce5c00; font-weight: bold">=</span><span style="color: #4e9a06">"test"</span>
<span style="color: #000000">test</span><span style="color: #ce5c00; font-weight: bold">=</span><span style="color: #000000">test</span><span style="color: #ce5c00; font-weight: bold">.</span><span style="color: #000000">replace</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #4e9a06">"test"</span><span style="color: #000000; font-weight: bold">,</span><span style="color: #4e9a06">""</span><span style="color: #000000; font-weight: bold">)</span>
<span style="color: #000000">x</span> <span style="color: #ce5c00; font-weight: bold">=</span> <span style="color: #204a87; font-weight: bold">True</span>
<span style="color: #204a87">print</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #4e9a06">"Done"</span> <span style="color: #204a87; font-weight: bold">if</span> <span style="color: #000000; font-weight: bold">(</span><span style="color: #000000">x</span> <span style="color: #204a87; font-weight: bold">if</span> <span style="color: #4e9a06">'x'</span> <span style="color: #204a87; font-weight: bold">in</span> <span style="color: #204a87">locals</span><span style="color: #000000; font-weight: bold">()</span> <span style="color: #204a87; font-weight: bold">else</span> <span style="color: #204a87; font-weight: bold">False</span><span style="color: #000000; font-weight: bold">)</span> <span style="color: #204a87; font-weight: bold">else</span> <span style="color: #4e9a06">"Failed"</span><span style="color: #000000; font-weight: bold">)</span>
<span style="color: #204a87; font-weight: bold">if</span> <span style="color: #4e9a06">'x'</span> <span style="color: #204a87; font-weight: bold">not</span> <span style="color: #204a87; font-weight: bold">in</span> <span style="color: #204a87">locals</span><span style="color: #000000; font-weight: bold">():</span>
  <span style="color: #204a87">print</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #4e9a06">'x is not defined'</span><span style="color: #000000; font-weight: bold">)</span>
</pre></div>

Yaml files used here<br>
[New syntax](https://github.com/LangTrans/Py_Trans/blob/main/source.yaml)(For token extraction)<br>
[Template of LISP](https://github.com/LangTrans/Py_Trans/blob/main/target.yaml)
### LISP
#### Customized Syntax of LISP

<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%;"><span></span><span style="color: #000000">func</span> <span style="color: #000000">printhis</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #000000">s</span><span style="color: #000000; font-weight: bold">):</span>
	<span style="color: #204a87">format</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #000000">t</span><span style="color: #000000; font-weight: bold">,</span><span style="color: #000000">s</span><span style="color: #000000; font-weight: bold">)</span>
<span style="color: #000000">printhis</span><span style="color: #000000; font-weight: bold">(</span><span style="color: #4e9a06">"Customized!"</span><span style="color: #000000; font-weight: bold">)</span>
</pre></div>

#### Original Syntax 
<div class="highlight" style="background: #f8f8f8"><pre style="line-height: 125%;"><span></span><span style="color: #000000; font-weight: bold">(</span><span style="color: #000000">defun</span> <span style="color: #000000">printhis</span> <span style="color: #000000; font-weight: bold">(</span><span style="color: #000000">s</span><span style="color: #000000; font-weight: bold">)</span>
	<span style="color: #000000; font-weight: bold">(</span><span style="color: #000000">format</span> <span style="color: #000000">t</span> <span style="color: #000000">s</span><span style="color: #000000; font-weight: bold">)</span>
<span style="color: #000000; font-weight: bold">)</span>
<span style="color: #000000; font-weight: bold">(</span><span style="color: #000000">printhis</span> <span style="color: #4e9a06">"Customized!"</span><span style="color: #000000; font-weight: bold">)</span>
</pre></div>

[New syntax](https://github.com/LangTrans/LangTrans/blob/main/example/source.yaml)<br>[Template of LISP](https://github.com/LangTrans/LangTrans/blob/main/example/target.yaml)
## Documentation
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
