---
title: 关于Markdown
date: 2021/11/13
description: 嗯
tag: web development
author: 驴哒
---

<div class="Post-body">
                    <h2>前言</h2>

<p>一个工具的精通需要的是长期的练习和使用， Markdown 语法也不例外，本文标题意在纠正大家对 Markdown 学习成本的错误高估以及消除大家对其的恐惧感。当然，只是读完本文五分钟还是足够的～</p>

<h2>正文</h2>

<h3>1. Markdown 是<em>什么</em>？</h3>

<p><strong>Markdown</strong> 是一种轻量级<strong>标记语言</strong>，它以纯文本形式<em>(易读、易写、易更改)</em>编写文档，并最终以<br>
 HTML 格式发布。</p>    

<h3>2. <em>谁</em>发明了这么个东西？</h3>

<p>它由 <a href="http://www.aaronsw.com/" rel=" nofollow ugc"><strong>Aaron Swartz</strong></a> 和 <strong>John Gruber</strong> 共同设计， <strong>Aaron Swartz</strong> 就是那位于不久前（<em>2013年1月11日</em>）自杀，有着<strong>开挂</strong>一般人生经历的程序员。维基百科对他的<a href="http://zh.wikipedia.org/wiki/%E4%BA%9A%E4%BC%A6%C2%B7%E6%96%AF%E6%B2%83%E8%8C%A8" rel=" nofollow ugc">介绍</a>是：<strong>软件工程师、作家、政治组织者、互联网活动家、维基百科人</strong>。</p>

<h3>3. <em>为什么</em>要使用它？</h3>

<ul><li>它易读<em>(看起来舒服)</em>、易写<em>(语法简单)</em>、易更改<em>(纯文本)</em>。处处体现着<strong>极简主义</strong>的影子。</li>
<li>兼容 HTML ，可以转换为 HTML 格式发布。</li>
<li>跨平台使用。</li>
<li>越来越多的网站支持 Markdown 。</li>
<li>更方便清晰的组织你的电子邮件。（Markdown-here, Airmail）</li>
<li>摆脱 Word（我不是认真的）。</li></ul>
 
<h3>4. <em>怎么</em>使用？</h3>

<p>如果不算<strong>扩展</strong>， Markdown 的语法绝对<strong>简单</strong>到让你爱不释手。</p>

<p>废话太多，下面正文， Markdown 语法主要分为如下几大部分：</p>

<p><strong>标题</strong>，<strong>段落</strong>，<strong>区块引用</strong>，<strong>代码区块</strong>，<strong>强调</strong>，<strong>列表</strong>，<strong>分割线</strong>，<strong>链接</strong>，<strong>图片</strong>，<strong>反斜杠 <code>\</code></strong>，<strong>符号'`'</strong>。</p>

<h4>4.1 标题</h4>

<p>两种形式：</p> 

<p>1）使用<code>=</code>和<code>-</code>标记一级和二级标题。</p>

<pre><code>一级标题   
=========
二级标题    
---------</code></pre>
  
<p>效果：</p>

<blockquote><h2>一级标题</h2>
<h2>二级标题</h2></blockquote>

<p>2）使用<code>#</code>，可表示1-6级标题。</p>

<pre><code># 一级标题   
## 二级标题   
### 三级标题   
#### 四级标题   
##### 五级标题   
###### 六级标题    </code></pre>

<p>效果：</p>

<blockquote><h1>一级标题</h1>
<h2>二级标题</h2>
<h3>三级标题</h3>
<h4>四级标题</h4>
<h5>五级标题</h5>
<h6>六级标题</h6></blockquote>

<h4>4.2 段落</h4>

<p>段落的前后要有空行，所谓的空行是指没有文字内容。若想在段内强制换行的方式是使用<strong>两个以上</strong>空格加上回车（引用中换行省略回车）。</p>

<h4>4.3 区块引用</h4>

<p>在段落的每行或者只在第一行使用符号<code>&gt;</code>,还可使用多个嵌套引用，如：</p>

<pre><code>&gt; 区块引用
&gt;&gt; 嵌套引用</code></pre>

<p>效果：</p>

<blockquote><p>区块引用</p>
<blockquote><p>嵌套引用</p></blockquote></blockquote>

<h4>4.4 代码区块</h4>

<p>代码区块的建立是在每行加上4个空格或者一个制表符（如同写代码一样）。如：</p>

<p>普通段落：</p>

<p>void main()    <br><br>
{    <br><br>
    printf("Hello, Markdown.");    <br><br>
}</p>    

<p>代码区块：</p>

<pre><code>void main()
{
    printf("Hello, Markdown.");
}</code></pre>

<p><strong>注意</strong>:需要和普通段落之间存在空行。</p>

<h4>4.5 强调</h4>

<p>在强调内容两侧分别加上<code>*</code>或者<code>_</code>，如：</p>

<pre><code> *斜体*，_斜体_  
 **粗体**，__粗体__</code></pre>


<p>效果：</p>

<blockquote><p><em>斜体</em>，<em>斜体</em>    <br><br>
<strong>粗体</strong>，<strong>粗体</strong></p></blockquote>

<h4>4.6 删去</h4>

<p>在表示被删去的内容两侧分别加上<code>~~</code>，如：</p>

<pre><code> ~~删除线~~</code></pre>

<p>效果：</p>

<blockquote><p><del>删除线</del></p> </blockquote>

<h4>4.7 列表</h4>

<p>使用<code>·</code>、<code>+</code>、或<code>-</code>标记无序列表，如：</p>

<pre><code>+ 第一项
+ 第二项
+ 第三项</code></pre>

<p><strong>注意</strong>：标记后面最少有一个<em>空格</em>或<em>制表符</em>。若不在引用区块中，必须和前方段落之间存在空行。</p>

<p>效果：</p>

<blockquote><ul><li>第一项</li>
<li>第二项</li>
<li>第三项</li></ul></blockquote>

<p>有序列表的标记方式是将上述的符号换成数字,并辅以<code>.</code>，如：</p>

<pre><code>1. 第一项   
2. 第二项    
3. 第三项    </code></pre>

<p>效果：</p>

<blockquote><ol><li>第一项</li>
<li>第二项</li>
<li>第三项</li></ol></blockquote>

<h4>4.8 分割线</h4>

<p>分割线最常使用就是三个或以上<code>*</code>，还可以使用<code>-</code>和<code>_</code>。</p>

<h4>4.9 链接</h4>

<p>链接可以由两种形式生成：<strong>行内式</strong>和<strong>参考式</strong>。</p> 
   <br>
<p><strong>行内式</strong>：</p>

<pre><code>[younghz的Markdown库](https://github.com/younghz/Markdown "Markdown")</code></pre>


<p>效果：</p>

<blockquote><p><a href="https://github.com/younghz/Markdown" rel=" nofollow ugc">younghz的Markdown库</a></p></blockquote>

<p><strong>参考式</strong>：</p>

<pre><code>[younghz的Markdown库1][1]    
[younghz的Markdown库2][2]    
[1]:https://github.com/younghz/Markdown "Markdown"    
[2]:https://github.com/younghz/Markdown "Markdown"    </code></pre>

<p>效果：</p>

<blockquote><p>[younghz的Markdown库1][1]<br>
[younghz的Markdown库2][2]</p></blockquote>

<h4>4.10 图片</h4>

<p>添加图片的形式和链接相似，只需在链接的基础上前方加一个叹号<code>!</code>。如：</p>

<pre><code>![Aaron Swartz](https://github.com/younghz/Markdown/raw/master/resource/Aaron_Swartz.jpg) </code></pre>

<p>效果：</p>

<blockquote><p><img src="https://github.com/younghz/Markdown/raw/master/resource/Aaron_Swartz.jpg" alt="Aaron Swartz"> <br>
（注：图示为 Markdown 创始人 Aaron Swartz）</p></blockquote>

<h4>4.11 反斜杠<code>\</code></h4>

<p>相当于<strong>反转义</strong>作用。使符号成为普通符号。</p>

<h4>4.12 符号'`'</h4>

<p>起到标记作用。如：</p>

<pre><code>`ctrl+a`</code></pre>


<p>效果：</p>

<blockquote><p><code>ctrl+a</code></p>    </blockquote>

<h4>5. 都<em>谁</em>在用？</h4>

<p>Markdown的使用者：</p>

<ul><li>GitHub</li>
<li>简书</li>
<li>Stack Overflow</li>
<li>Apollo</li>
<li>Moodle</li>
<li>Reddit</li>
<li>等等</li></ul>

<h4>6. 感觉有意思？趁热打铁，推荐几个<em>工具</em>。</h4>

<ul><li><strong>Chrome</strong> 下的 stackedit 插件可以离线使用，很爽。也不用担心平台受限。<br>
在线的 dillinger.io 算是评价好的了，可是不能离线使用。    </li>
<li><strong>Windowns</strong> 下目前我在使用 Typora ，感觉挺棒，同时它也是 <strong>跨平台</strong> 的，其他平台用户也可以尝试一下。</li>
<li><strong>Mac</strong> 下的 Mou 是国人贡献的，口碑很好。推荐。    </li>
<li><strong>Linux</strong> 下的 ReText 不错。    </li></ul>

<p><strong>其实对语法了然于心的话，直接用纯文本编辑器就可以了，脑子里满满的都是格式化好的文本啊。</strong></p>

<hr>
<p><strong>注意</strong>：不同的 Markdown 解释器或工具对相应语法（扩展语法）的解释效果不尽相同，具体可参见工具的使用说明。<br>
虽然有人想出面搞一个所谓的标准化的Markdown，<a href="http://blog.codinghorror.com/standard-markdown-is-now-common-markdown/" rel=" nofollow ugc">没想到还惹怒了健在的创始人John Gruber</a>。</p>
<hr>

<p>以上基本是所有 Traditonal Markdown 的语法。</p>

<h3>其它：</h3>

<p>列表的使用（非 Traditonal Markdown ）：</p>

<p>用<code>|</code>表示表格纵向边界，表头和表内容用<code>-</code>隔开，并可用<code>:</code>进行对齐设置，两边都有<code>:</code>则表示居中，若不加<code>:</code>则默认左对齐。</p>

<blockquote><p>|代码库                              |链接                                |<br>
|:------------------------------------😐------------------------------------|<br>
|MarkDown                              | <a href="https://github.com/younghz/Markdown" rel=" nofollow ugc">https://github.com/younghz/Markdown</a>|<br>
|moos-young                            |<a href="https://github.com/younghz/moos-young" rel=" nofollow ugc">https://github.com/younghz/moos-young</a>|</p></blockquote>

<p>关于其它扩展语法可参见具体工具的使用说明。</p>

<h3>我该在哪里试试它呢？</h3>

<p>最简单的就是找一个支持 Markdown 的在线 pastebin 类站点，例如 <a href="https://gist.github.com" rel=" nofollow ugc">Github Gist</a> (注:在大陆可能被屏蔽) 。你也可以在这个帖子直接回复测试 Markdown 语法，请直接编辑你的回复做更多测试。注意：不要在此帖外的任何地方发表无意义的语法测试内容！</p>
                </div>
            </div>
            
