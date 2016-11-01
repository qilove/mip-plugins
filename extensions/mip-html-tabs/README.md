# **mip-html-tabs**
mip-html-tabs TAB滑动、显示、隐藏等操作。
<table><thead>
<tr>
<th>描述</th>
<th>提供用来支持页面点击显示隐藏、TAB切换、返回顶部等操作。</th>
</tr>
</thead><tbody>
<tr>
<td>可用性</td>
<td>完成</td>
</tr>
<tr>
<td>所需脚本</td>
<td>mip-html-tabs.js</td>
</tr>
</tbody></table>

## 1.使用

- Qi_1 当内容高度大于设置高度后展开、隐藏操作。

`<mip-html-tabs tabs-type="Qi_1" tabs-html="#hidebox" tabs-height="200" tabs-show=".tabs-show" tabs-hide=".tabs-hide"><div id="hidebox">超过隐藏部分内容（默认高度300px）</div><span class="tabs-show">展开全部</span><span class="tabs-hide">收起简介</span></mip-html-tabs>`

- Qi_2 设置一个点击元素，执行toggle显示隐藏操作。

`<mip-html-tabs tabs-type="Qi_2" tabs-on="#Isck" tabs-toggle="#Istoggle1"><div id="Istoggle1"><h2>内容1</h2>内容1</div><div id="Isck">点击显示或隐藏内容1</div></mip-html-tabs>`

- Qi_3 设置两个点击元素，执行显示隐藏操作。

`<mip-html-tabs tabs-type="Qi_3" tabs-show="#Isshow2" tabs-hide="#Ishide2" tabs-toggle="#Istoggle2"><div id="Istoggle2"><h2>内容2</h2>内容2</div><div id="Isshow2">点击显示内容2</div><div id="Ishide2">点击隐藏内容2</div></mip-html-tabs>`

- Qi_4 Tab内容切换。

`<mip-html-tabs tabs-type="Qi_4" tabs-nav="#nav1 ul li" tabs-key="#tab1 ul"><div id="nav1"><ul><li>Tab1</li><li>Tab2</li><li>Tab3</li><li>Tab4</li></ul></div><div id="tab1"><ul><li>Tab1 html</li></ul><ul><li>Tab2 html</li></ul><ul><li>Tab3 html</li></ul><ul><li>Tab4 html</li></ul></div></mip-html-tabs>`

- Qi_5 点击元素滚动事件。

`<mip-html-tabs tabs-type="Qi_5" tabs-key="#Istop" tabs-to="top"><div id="Istop">返回顶部</div></mip-html-tabs>`

## 2.属性

<ul><li>tabs-type<ul>
<li>是否必填：是</li>
<li>属性说明：Qi_1、Qi_2、Qi_3、Qi_4、Qi_5，五中方法</li>
</ul></li></ul>

### tabs-type：Qi_1
<ul><li>tabs-html<ul>
<li>是否必填：是</li>
<li>属性说明：指定超过高度需要隐藏的元素</li>
</ul></li></ul>
<ul><li>tabs-height<ul>
<li>是否必填：否</li>
<li>属性说明：指定高度px值，默认300</li>
</ul></li></ul>
<ul><li>tabs-show<ul>
<li>是否必填：是</li>
<li>属性说明：指定展开按钮元素</li>
</ul></li></ul>
<ul><li>tabs-hide<ul>
<li>是否必填：是</li>
<li>属性说明：指定收起按钮元素</li>
</ul></li></ul>
<ul><li>tabs-init<ul>
<li>是否必填：否</li>
<li>属性说明：0：默认隐藏，1：默认显示，默认：0</li>
</ul></li></ul>

### tabs-type：Qi_2
<ul><li>tabs-toggle<ul>
<li>是否必填：是</li>
<li>属性说明：指定显示隐藏元素</li>
</ul></li></ul>
<ul><li>tabs-on<ul>
<li>是否必填：是</li>
<li>属性说明：指定点击按钮元素</li>
</ul></li></ul>
<ul><li>tabs-init<ul>
<li>是否必填：否</li>
<li>属性说明：0：默认隐藏，1：默认显示，默认：0</li>
</ul></li></ul>

### tabs-type：Qi_3
<ul><li>tabs-toggle<ul>
<li>是否必填：是</li>
<li>属性说明：指定显示隐藏元素</li>
</ul></li></ul>
<ul><li>tabs-on<ul>
<li>是否必填：是</li>
<li>属性说明：指定点击按钮元素</li>
</ul></li></ul>
<ul><li>tabs-init<ul>
<li>是否必填：否</li>
<li>属性说明：0：默认隐藏，1：默认显示，默认：0</li>
</ul></li></ul>

### tabs-type：Qi_4
<ul><li>tabs-nav<ul>
<li>是否必填：是</li>
<li>属性说明：指定TAB按钮元素</li>
</ul></li></ul>
<ul><li>tabs-key<ul>
<li>是否必填：是</li>
<li>属性说明：指定TAB内容元素</li>
</ul></li></ul>
<ul><li>tabs-init<ul>
<li>是否必填：否</li>
<li>属性说明：数值，默认显示TAB:n内容</li>
</ul></li></ul>
<ul><li>nav-cur<ul>
<li>是否必填：否</li>
<li>属性说明：当前TAB按钮class</li>
</ul></li></ul>
<ul><li>key-cur<ul>
<li>是否必填：否</li>
<li>属性说明：当前TAB内容class</li>
</ul></li></ul>

### tabs-type：Qi_5
<ul><li>tabs-key<ul>
<li>是否必填：是</li>
<li>属性说明：点击按钮元素</li>
</ul></li></ul>
<ul><li>tabs-to<ul>
<li>是否必填：是</li>
<li>属性说明：top：跳到顶部，bottom：跳到底部，(元素)：跳到指定元素</li>
</ul></li></ul>
<ul><li>tabs-on<ul>
<li>是否必填：否</li>
<li>属性说明：点击事件元素</li>
</ul></li></ul>
<ul><li>tabs-eq<ul>
<li>是否必填：否</li>
<li>属性说明：点击事件元素eq</li>
</ul></li></ul>
<ul><li>tabs-top<ul>
<li>是否必填：否</li>
<li>属性说明：数值，按钮元素超过tabs-top后值显示</li>
</ul></li></ul>
<ul><li>tabs-of<ul>
<li>是否必填：否</li>
<li>属性说明：数值，tabs-to的偏移可负数</li>
</ul></li></ul>
