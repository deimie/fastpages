---
keywords: fastai
title: Array List Lesson
image: images/javaLogo.png
nb_path: _notebooks/2022-10-07-array-list.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2022-10-07-array-list.ipynb
-->

<div class="container" id="notebook-container">
        
    {% raw %}
    
<div class="cell border-box-sizing code_cell rendered">
<div class="input">

<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-java"><pre><span></span><span class="kn">import</span> <span class="nn">java.util.Arrays</span><span class="p">;</span>
<span class="kn">import</span> <span class="nn">java.util.ArrayList</span><span class="p">;</span>

<span class="kd">public</span> <span class="kd">class</span> <span class="nc">arrayListLesson</span> <span class="p">{</span>

    <span class="kd">public</span> <span class="kd">static</span> <span class="kt">void</span> <span class="nf">main</span><span class="p">(</span><span class="n">String</span><span class="o">[]</span> <span class="n">args</span><span class="p">)</span> <span class="p">{</span>

        <span class="n">ArrayList</span><span class="o">&lt;</span><span class="n">String</span><span class="o">&gt;</span> <span class="n">myArray</span> <span class="o">=</span> <span class="k">new</span> <span class="n">ArrayList</span><span class="o">&lt;&gt;</span><span class="p">(</span><span class="n">Arrays</span><span class="p">.</span><span class="na">asList</span><span class="p">(</span><span class="s">&quot;Index1&quot;</span><span class="p">,</span> <span class="s">&quot;Index2&quot;</span><span class="p">,</span> <span class="s">&quot;Index3&quot;</span><span class="p">,</span> <span class="s">&quot;Index4&quot;</span><span class="p">));</span>

        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">myArray</span><span class="p">);</span> <span class="c1">// print entire list</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">myArray</span><span class="p">.</span><span class="na">get</span><span class="p">(</span><span class="mi">1</span><span class="p">));</span> <span class="c1">// print index 1 (starting at 0 of course)</span>

        <span class="n">myArray</span><span class="p">.</span><span class="na">add</span><span class="p">(</span><span class="s">&quot;Index5&quot;</span><span class="p">);</span>
        <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="n">myArray</span><span class="p">);</span>

        <span class="k">if</span><span class="p">(</span><span class="n">myArray</span><span class="p">.</span><span class="na">contains</span><span class="p">(</span><span class="s">&quot;Index4&quot;</span><span class="p">))</span> <span class="p">{</span> <span class="c1">// .contains checks if an index exists</span>
            <span class="n">System</span><span class="p">.</span><span class="na">out</span><span class="p">.</span><span class="na">println</span><span class="p">(</span><span class="s">&quot;Index 4 exists.&quot;</span><span class="p">);</span>
        <span class="p">}</span>
    <span class="p">}</span>
<span class="p">}</span>


<span class="n">arrayListLesson</span><span class="p">.</span><span class="na">main</span><span class="p">(</span><span class="kc">null</span><span class="p">);</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>[Index1, Index2, Index3, Index4]
Index2
[Index1, Index2, Index3, Index4, Index5]
Index 4 exists.
</pre>
</div>
</div>

</div>
</div>

</div>
    {% endraw %}

</div>
 

