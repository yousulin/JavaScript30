<h1>完成目標</h1>
<p>一個鍵盤爵士鼓</p>
<ul>
  <li>功能</li>
  <ul>
    <li>按下鍵盤，出現相對應的聲音</li>
  </ul>
  <li>畫面</li>
  <ul>
    <li>按下鍵盤，畫面上的字母方塊，做點小動畫</li>
    <ul>
      <li>加上黃色陰影</li>
      <li>按鈕彈一下(微小放大)的動畫</li>
    </ul>
  </ul>
 </ul>
<h1>Javascript</h1>
<h2>Arrow Function</h2>
<ul>
<li>
  <a href="http://www.jollen.org/blog/2013/10/javascript-lambda.html" rel="nofollow">lambda</a> 在Javascript裡叫 <code>arrow function</code></li>
</ul>
<p>一般js的匿名函數這樣寫</p>
<div class="snippet-clipboard-content position-relative" data-snippet-clipboard-copy-content="funtion (key) {
  key.addEventListener('transitionend', removeTransition);
}
"><pre lang="javascript="><code>funtion (key) {
  key.addEventListener('transitionend', removeTransition);
}
</code></pre></div>
<p>用<code>arrow function</code>的寫法就是</p>
<div class="snippet-clipboard-content position-relative" data-snippet-clipboard-copy-content="key =&gt; key.addEventListener('transitionend', removeTransition)
"><pre lang="javascript="><code>key =&gt; key.addEventListener('transitionend', removeTransition)
</code></pre></div>
<blockquote>
<p>不同之處在於<code>this</code>，一般的寫法有<code>this</code>=<code>function</code>本身，但是「誰」呼叫<code>arrow function</code>，「誰」=<code>this</code>。</p>
</blockquote>
<h2>Window方法</h2>
<p>jsref: <a href="https://www.w3schools.com/jsref/obj_window.asp" rel="nofollow">The Window Object</a></p>
<ul>
<li><a href="https://www.w3schools.com/jsref/met_win_settimeout.asp" rel="nofollow"><code>setTimeout(function, ms)</code></a> 設定「執行一次」的function與延遲時間</li>
</ul>
<h2>DOM Document 方法</h2>
<p>jsref: <a href="https://www.w3schools.com/jsref/dom_obj_document.asp" rel="nofollow">The HTML DOM Document Object</a></p>
<ul>
<li><code>document.querySelector()</code>找到第一個符合指定CSS selector(s)的HTML節點</li>
<li><code>document.querySelectorAll()</code>找到符合指定CSS selector(s)的HTML節點們</li>
</ul>
<h2>DOM Element 方法</h2>
<p>jsref: <a href="https://www.w3schools.com/jsref/dom_obj_all.asp" rel="nofollow">The HTML DOM Element Object</a></p>
<ul>
<li><code>element.addEventListener()</code> 加一個事件到Element上</li>
<li><code>element.classList</code> 回傳NodeList，element上的class屬性的內容</li>
</ul>
<h2>NodeList 方法</h2>
<p>jsref: <a href="https://www.w3schools.com/js/js_htmldom_nodelist.asp" rel="nofollow">JavaScript HTML DOM Node List</a></p>
<ul>
<li><code>NodeList.forEach()</code></li>
</ul>
<p><code>querySelectorAll()</code>出來的物件都是<code>NodeList</code>，它不是<code>Array</code>，能使用的方法不同，在此使用<code>forEach()</code>走訪每一個元素。</p>
<p>參考: <a href="https://www.w3schools.com/jsref/jsref_forEach.asp" rel="nofollow"><code>Array.forEach</code></a></p>
<h2>Event Object 方法</h2>
<p>jsref: <a href="https://www.w3schools.com/jsref/dom_obj_event.asp" rel="nofollow">HTML DOM Events</a></p>
<ul>
<li><a href="https://www.w3schools.com/jsref/event_transitionend.asp" rel="nofollow"><code>Transition Events</code></a> 過場結束(transition end)執行 myFunction</li>
</ul>
<p>「過場」唯一事件</p>
<div class="snippet-clipboard-content position-relative" data-snippet-clipboard-copy-content="element.addEventListener(&quot;transitionend&quot;, myFunction)
"><pre lang="javascript="><code>element.addEventListener("transitionend", myFunction)
</code></pre></div>
