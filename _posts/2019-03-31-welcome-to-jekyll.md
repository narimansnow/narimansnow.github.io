---
layout: post
title:  "Контакты"
date:   2019-03-13 12:01:13 +0300
category: news
---
<li>------------------------------------------------------------------------------------</li>
<li>Город:              Саров</li>
<li>Место учёбы:        СарФТИ НИЯУ МИФИ</li>
<li>------------------------------------------------------------------------------------</li>
<li>Моб. телефон: 89151563490</li>
<li>Дом. телефон: 88344527390</li>
<li>Skype: nariman7189</li>
<li>-------------------------------------------------------------------------------------</li>


<div class="language-css highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nf">#include</span> <span class="o">&lt;</span><span class="nt">iostream</span><span class="o">&gt;</span>
<span class="nf">#include</span> <span class="o">&lt;</span><span class="nt">typeinfo</span><span class="o">&gt;</span>

<span class="nt">class</span> <span class="nt">myTypeA</span><span class="p">{}</span><span class="o">;</span>
<span class="nt">class</span> <span class="nt">myTypeB</span> <span class="o">:</span> <span class="nt">public</span> <span class="nt">myTypeA</span> <span class="p">{}</span><span class="o">;</span>
<span class="nt">class</span> <span class="nt">myTypeC</span> <span class="o">:</span> <span class="nt">public</span> <span class="nt">myTypeB</span> <span class="p">{}</span><span class="o">;</span>

<span class="nt">int</span> <span class="nt">main</span><span class="o">()</span> <span class="p">{</span>
    <span class="err">myTypeA</span> <span class="err">*obj1</span> <span class="err">=</span> <span class="err">new</span> <span class="err">myTypeA;</span>
    <span class="err">myTypeA</span> <span class="err">*obj2</span> <span class="err">=</span> <span class="err">new</span> <span class="err">myTypeB;</span>
    <span class="err">myTypeA</span> <span class="err">*obj3</span> <span class="err">=</span> <span class="err">new</span> <span class="err">myTypeC;</span>

    <span class="err">myTypeB</span> <span class="err">*obj4</span> <span class="err">=</span> <span class="err">new</span> <span class="err">myTypeB;</span>
    <span class="err">myTypeB</span> <span class="err">*obj5</span> <span class="err">=</span> <span class="err">new</span> <span class="err">myTypeC;</span>

    <span class="err">myTypeC</span> <span class="err">*obj6</span> <span class="err">=</span> <span class="err">new</span> <span class="err">myTypeC;</span>

    <span class="py">std</span><span class="p">::</span><span class="n">cout</span> <span class="err">&lt;&lt;</span> <span class="n">typeid</span><span class="p">(</span><span class="n">obj1</span><span class="p">).</span><span class="n">name</span><span class="p">();</span>
    <span class="py">std</span><span class="p">::</span><span class="n">cout</span> <span class="err">&lt;&lt;</span> <span class="n">typeid</span><span class="p">(</span><span class="n">obj2</span><span class="p">).</span><span class="n">name</span><span class="p">();</span>
    <span class="py">std</span><span class="p">::</span><span class="n">cout</span> <span class="err">&lt;&lt;</span> <span class="n">typeid</span><span class="p">(</span><span class="n">obj3</span><span class="p">).</span><span class="n">name</span><span class="p">();</span>
    <span class="py">std</span><span class="p">::</span><span class="n">cout</span> <span class="err">&lt;&lt;</span> <span class="n">typeid</span><span class="p">(</span><span class="n">obj4</span><span class="p">).</span><span class="n">name</span><span class="p">();</span>
    <span class="py">std</span><span class="p">::</span><span class="n">cout</span> <span class="err">&lt;&lt;</span> <span class="n">typeid</span><span class="p">(</span><span class="n">obj5</span><span class="p">).</span><span class="n">name</span><span class="p">();</span>
    <span class="py">std</span><span class="p">::</span><span class="n">cout</span> <span class="err">&lt;&lt;</span> <span class="n">typeid</span><span class="p">(</span><span class="n">obj6</span><span class="p">).</span><span class="n">name</span><span class="p">();</span>
<span class="p">}</span>
</code></pre></div></div>


<div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="kn">import</span> <span class="nn">csv</span>
<span class="n">authorsEmail</span> <span class="o">=</span> <span class="p">{}</span>
<span class="k">with</span> <span class="nb">open</span><span class="p">(</span> <span class="s">"calculator.history"</span><span class="p">,</span> <span class="s">"rt"</span> <span class="p">)</span> <span class="k">as</span> <span class="nb">file</span><span class="p">:</span>
    <span class="n">reader</span> <span class="o">=</span> <span class="n">csv</span><span class="o">.</span><span class="n">reader</span><span class="p">(</span> <span class="nb">file</span> <span class="p">)</span>
    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">reader</span><span class="p">:</span>
        <span class="n">name</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
        <span class="n">email</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>
        <span class="k">if</span> <span class="n">name</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">authorsEmail</span><span class="p">:</span>
            <span class="n">authorsEmail</span><span class="p">[</span> <span class="n">name</span> <span class="p">]</span> <span class="o">=</span> <span class="p">[]</span>
        <span class="n">emailList</span> <span class="o">=</span> <span class="n">authorsEmail</span><span class="p">[</span> <span class="n">name</span> <span class="p">]</span>
        <span class="k">if</span> <span class="n">email</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">emailList</span><span class="p">:</span>
            <span class="n">emailList</span><span class="o">.</span><span class="n">append</span><span class="p">(</span> <span class="n">email</span> <span class="p">)</span>
<span class="k">for</span> <span class="n">name</span><span class="p">,</span> <span class="n">email</span> <span class="ow">in</span> <span class="n">authorsEmail</span><span class="o">.</span><span class="n">items</span><span class="p">():</span>
    <span class="k">print</span> <span class="n">name</span><span class="p">,</span> <span class="n">email</span>
</code></pre></div></div>
