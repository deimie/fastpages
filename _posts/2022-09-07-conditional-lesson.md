---
keywords: fastai
title: Java Conditionals
image: images/javaLogo.png
nb_path: _notebooks/2022-09-07-conditional-lesson.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-09-07-conditional-lesson.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="c1">// De Morgan&#39;s Law Demonstration </span>

<span class="k">if</span> <span class="p">(</span><span class="o">!</span><span class="p">(</span><span class="kc">true</span> <span class="o">&amp;&amp;</span> <span class="kc">false</span><span class="p">))</span> <span class="p">{</span> <span class="c1">// if NOT (true AND false)</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;1st True&quot;</span><span class="p">);</span>
<span class="p">}</span>

<span class="k">if</span> <span class="p">(</span><span class="kc">false</span> <span class="o">||</span> <span class="kc">true</span><span class="p">)</span> <span class="p">{</span> <span class="c1">//simplfied version of above condition. if false OR true</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;2nd True&quot;</span><span class="p">);</span>
<span class="p">}</span>

<span class="cm">/* According to De Morgan&#39;s law, a NOT condition will turn an AND into an OR and an OR into an AND. </span>
<span class="cm">The two conditon above are the same condition. */</span>

<span class="k">if</span> <span class="p">(</span><span class="o">!</span><span class="p">(</span><span class="kc">false</span> <span class="o">&amp;&amp;</span> <span class="o">!</span><span class="kc">false</span><span class="p">))</span> <span class="p">{</span> <span class="c1">// if NOT (false AND NOT(false))</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;3rd True&quot;</span><span class="p">);</span>
<span class="p">}</span>

<span class="k">if</span> <span class="p">(</span><span class="kc">true</span> <span class="o">||</span> <span class="kc">true</span><span class="p">)</span> <span class="p">{</span> <span class="c1">// simplified version of above condition. if true OR true</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;4th True&quot;</span><span class="p">);</span>
<span class="p">}</span>

<span class="k">if</span> <span class="p">(</span><span class="o">!</span><span class="p">(</span><span class="kc">true</span> <span class="o">||</span> <span class="kc">true</span><span class="p">))</span> <span class="p">{</span> <span class="c1">// this last one does not display because the OR switches to an AND and the trues switch to falses</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;5th True&quot;</span><span class="p">);</span>
<span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>1st True
2nd True
3rd True
4th True
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="c1">// If, Else If, Else Demonstration</span>

<span class="k">if</span> <span class="p">(</span><span class="mi">1</span> <span class="o">==</span> <span class="mi">1</span><span class="p">)</span> <span class="p">{</span> <span class="c1">// if 1 is 1 (it always is) display true</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;This is true&quot;</span><span class="p">);</span>
<span class="p">}</span>

<span class="k">if</span> <span class="p">(</span><span class="mi">1</span> <span class="o">==</span> <span class="mi">2</span><span class="p">)</span> <span class="p">{</span> <span class="c1">// 1 is not 2 so this is ignored</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;This won&#39;t display&quot;</span><span class="p">);</span>
<span class="p">}</span> 
<span class="k">else</span> <span class="k">if</span> <span class="p">(</span><span class="mi">2</span> <span class="o">==</span> <span class="mi">2</span><span class="p">){</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;This one&#39;s also true&quot;</span><span class="p">);</span>

<span class="p">}</span>

<span class="k">if</span> <span class="p">(</span><span class="mi">1</span> <span class="o">==</span> <span class="mi">2</span><span class="p">)</span> <span class="p">{</span> <span class="c1">// Non-true statement</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;This isn&#39;t true&quot;</span><span class="p">);</span>
<span class="p">}</span>
<span class="k">else</span> <span class="k">if</span> <span class="p">(</span><span class="mi">1</span> <span class="o">==</span> <span class="mi">3</span><span class="p">)</span> <span class="p">{</span> <span class="c1">// Non-true statement</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;This isn&#39;t either&quot;</span><span class="p">);</span>
<span class="p">}</span>
<span class="k">else</span> <span class="p">{</span> <span class="c1">// Because no other statements were true, this is the last response</span>
    <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Nothing else was true, so this is the reponse if nothing else works.&quot;</span><span class="p">);</span>
<span class="p">}</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>This is true
This one&#39;s also true
Nothing else was true, so this is the reponse if nothing else works.
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

