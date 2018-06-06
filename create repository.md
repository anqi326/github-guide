---


---

<h2 id="创建版本库">创建版本库</h2>
<h3 id="创建一个空目录">1. 创建一个空目录</h3>
<pre class=" language-bash"><code class="prism  language-bash">$ <span class="token function">mkdir</span> repository
$ <span class="token function">cd</span> repository
</code></pre>
<h3 id="把目录变成git仓库">2. 把目录变成git仓库</h3>
<pre class=" language-bash"><code class="prism  language-bash">$ <span class="token function">git</span> init
$ Initialized empty Git repository <span class="token keyword">in</span> C:/Users/uidw3549/Git/02.Github Repository/repository/.git/
</code></pre>
<h3 id="编写新文件">3. 编写新文件</h3>
<pre class=" language-bash"><code class="prism  language-bash">$ <span class="token keyword">echo</span> <span class="token string">"this is readme file"</span> <span class="token operator">&gt;</span> readme.txt
$ <span class="token function">ls</span>
readme.txt
</code></pre>
<h3 id="添加文件到仓库">4. 添加文件到仓库</h3>
<p>添加文件到<a href="/staging">暂存区</a> 	<br>
<code>bash 	$ git add readme.txt</code></p>
<p>查看仓库状态</p>
<pre class=" language-bash"><code class="prism  language-bash"> $ <span class="token function">git</span> status
 On branch master
 Initial commit
 Changes to be committed:
 	<span class="token punctuation">(</span>use <span class="token string">"git rm --cached &lt;file&gt;..."</span> to unstage<span class="token punctuation">)</span>
 	   new file:   readme.txt
</code></pre>
<p>提交到仓库</p>
<pre class=" language-bash"><code class="prism  language-bash">$ <span class="token function">git</span> commit -m<span class="token string">"create readme.txt"</span>
<span class="token punctuation">[</span>master <span class="token punctuation">(</span>root-commit<span class="token punctuation">)</span> d9abbb7<span class="token punctuation">]</span> create readme.txt
 1 <span class="token function">file</span> changed, 1 insertion<span class="token punctuation">(</span>+<span class="token punctuation">)</span>
 create mode 100644 readme.txt
</code></pre>
<p>再查看文件状态,文件已经提交到仓库中</p>
<pre class=" language-bash"><code class="prism  language-bash">$ <span class="token function">git</span> status
On branch master
nothing to commit, working tree clean
</code></pre>
<hr>
<ul>
<li><code>$ git init</code> 创建创建仓库</li>
<li><code>$ git add &lt;file&gt;</code> 添加文件到暂存区</li>
<li><code>$ git commit -m &lt;message&gt;</code> 提交到仓库</li>
<li><code>$ git status</code> 查看仓库状态</li>
</ul>

