---
title: Chapter 2. Homotopy Type Theory - Exercises
---

# Chapter 2. Homotopy Type Theory - Exercises

<pre class="Agda"><a id="116" class="Keyword">module</a> <a id="123" href="Chapter2.Exercises.html" class="Module">Chapter2.Exercises</a> <a id="142" class="Keyword">where</a>

<a id="149" class="Keyword">open</a> <a id="154" class="Keyword">import</a> <a id="161" href="Chapter2.Book.html" class="Module">Chapter2.Book</a> <a id="175" class="Keyword">public</a>

<a id="183" class="Comment">-- Exercise 2.10</a>
<a id="Σ-assoc"></a><a id="200" href="Chapter2.Exercises.html#200" class="Function">Σ-assoc</a> <a id="208" class="Symbol">:</a> <a id="210" class="Symbol">{</a><a id="211" href="Chapter2.Exercises.html#211" class="Bound">A</a> <a id="213" class="Symbol">:</a> <a id="215" href="Chapter1.Book.html#345" class="Function">𝒰</a> <a id="217" href="Chapter1.Book.html#328" class="Generalizable">𝒾</a><a id="218" class="Symbol">}</a> <a id="220" class="Symbol">{</a><a id="221" href="Chapter2.Exercises.html#221" class="Bound">B</a> <a id="223" class="Symbol">:</a> <a id="225" href="Chapter2.Exercises.html#211" class="Bound">A</a> <a id="227" class="Symbol">→</a> <a id="229" href="Chapter1.Book.html#345" class="Function">𝒰</a> <a id="231" href="Chapter1.Book.html#330" class="Generalizable">𝒿</a><a id="232" class="Symbol">}</a> <a id="234" class="Symbol">(</a><a id="235" href="Chapter2.Exercises.html#235" class="Bound">C</a> <a id="237" class="Symbol">:</a> <a id="239" class="Symbol">(</a><a id="240" href="Chapter1.Book.html#1550" class="Function">Σ</a> <a id="242" href="Chapter2.Exercises.html#242" class="Bound">x</a> <a id="244" href="Chapter1.Book.html#1550" class="Function">꞉</a> <a id="246" href="Chapter2.Exercises.html#211" class="Bound">A</a> <a id="248" href="Chapter1.Book.html#1550" class="Function">,</a> <a id="250" href="Chapter2.Exercises.html#221" class="Bound">B</a> <a id="252" href="Chapter2.Exercises.html#242" class="Bound">x</a><a id="253" class="Symbol">)</a> <a id="255" class="Symbol">→</a> <a id="257" href="Chapter1.Book.html#345" class="Function">𝒰</a> <a id="259" href="Chapter1.Book.html#332" class="Generalizable">𝓀</a><a id="260" class="Symbol">)</a>
        <a id="270" class="Symbol">→</a> <a id="272" class="Symbol">(</a><a id="273" href="Chapter1.Book.html#1550" class="Function">Σ</a> <a id="275" href="Chapter2.Exercises.html#275" class="Bound">x</a> <a id="277" href="Chapter1.Book.html#1550" class="Function">꞉</a> <a id="279" href="Chapter2.Exercises.html#211" class="Bound">A</a> <a id="281" href="Chapter1.Book.html#1550" class="Function">,</a> <a id="283" class="Symbol">(</a><a id="284" href="Chapter1.Book.html#1550" class="Function">Σ</a> <a id="286" href="Chapter2.Exercises.html#286" class="Bound">y</a> <a id="288" href="Chapter1.Book.html#1550" class="Function">꞉</a> <a id="290" href="Chapter2.Exercises.html#221" class="Bound">B</a> <a id="292" href="Chapter2.Exercises.html#275" class="Bound">x</a> <a id="294" href="Chapter1.Book.html#1550" class="Function">,</a> <a id="296" href="Chapter2.Exercises.html#235" class="Bound">C</a> <a id="298" class="Symbol">(</a><a id="299" href="Chapter2.Exercises.html#275" class="Bound">x</a> <a id="301" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="303" href="Chapter2.Exercises.html#286" class="Bound">y</a><a id="304" class="Symbol">)))</a> <a id="308" href="Chapter2.Book.html#8761" class="Function Operator">≃</a> <a id="310" class="Symbol">(</a><a id="311" href="Chapter1.Book.html#1550" class="Function">Σ</a> <a id="313" href="Chapter2.Exercises.html#313" class="Bound">p</a> <a id="315" href="Chapter1.Book.html#1550" class="Function">꞉</a> <a id="317" class="Symbol">(</a><a id="318" href="Chapter1.Book.html#1550" class="Function">Σ</a> <a id="320" href="Chapter2.Exercises.html#320" class="Bound">x</a> <a id="322" href="Chapter1.Book.html#1550" class="Function">꞉</a> <a id="324" href="Chapter2.Exercises.html#211" class="Bound">A</a> <a id="326" href="Chapter1.Book.html#1550" class="Function">,</a> <a id="328" href="Chapter2.Exercises.html#221" class="Bound">B</a> <a id="330" href="Chapter2.Exercises.html#320" class="Bound">x</a><a id="331" class="Symbol">)</a> <a id="333" href="Chapter1.Book.html#1550" class="Function">,</a> <a id="335" href="Chapter2.Exercises.html#235" class="Bound">C</a> <a id="337" href="Chapter2.Exercises.html#313" class="Bound">p</a><a id="338" class="Symbol">)</a>
<a id="340" href="Chapter2.Exercises.html#200" class="Function">Σ-assoc</a> <a id="348" href="Chapter2.Exercises.html#348" class="Bound">C</a> <a id="350" class="Symbol">=</a> <a id="352" href="Chapter2.Exercises.html#399" class="Function">map</a> <a id="356" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="358" href="Chapter2.Book.html#8273" class="Function">invs⇒equivs</a> <a id="370" href="Chapter2.Exercises.html#399" class="Function">map</a> <a id="374" class="Symbol">(</a><a id="375" href="Chapter2.Exercises.html#437" class="Function">map⁻¹</a> <a id="381" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="383" href="Chapter2.Exercises.html#477" class="Function">ε</a> <a id="385" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="387" href="Chapter2.Exercises.html#488" class="Function">η</a><a id="388" class="Symbol">)</a>
 <a id="391" class="Keyword">where</a>
  <a id="399" href="Chapter2.Exercises.html#399" class="Function">map</a> <a id="403" class="Symbol">=</a> <a id="405" class="Symbol">λ</a> <a id="407" class="Symbol">(</a><a id="408" href="Chapter2.Exercises.html#408" class="Bound">x</a> <a id="410" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="412" href="Chapter2.Exercises.html#412" class="Bound">y</a> <a id="414" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="416" href="Chapter2.Exercises.html#416" class="Bound">c</a><a id="417" class="Symbol">)</a> <a id="419" class="Symbol">→</a> <a id="421" class="Symbol">((</a><a id="423" href="Chapter2.Exercises.html#408" class="Bound">x</a> <a id="425" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="427" href="Chapter2.Exercises.html#412" class="Bound">y</a><a id="428" class="Symbol">)</a> <a id="430" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="432" href="Chapter2.Exercises.html#416" class="Bound">c</a><a id="433" class="Symbol">)</a>
  <a id="437" href="Chapter2.Exercises.html#437" class="Function">map⁻¹</a> <a id="443" class="Symbol">=</a> <a id="445" class="Symbol">λ</a> <a id="447" class="Symbol">((</a><a id="449" href="Chapter2.Exercises.html#449" class="Bound">x</a> <a id="451" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="453" href="Chapter2.Exercises.html#453" class="Bound">y</a><a id="454" class="Symbol">)</a> <a id="456" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="458" href="Chapter2.Exercises.html#458" class="Bound">c</a><a id="459" class="Symbol">)</a> <a id="461" class="Symbol">→</a> <a id="463" class="Symbol">(</a><a id="464" href="Chapter2.Exercises.html#449" class="Bound">x</a> <a id="466" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="468" href="Chapter2.Exercises.html#453" class="Bound">y</a> <a id="470" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="472" href="Chapter2.Exercises.html#458" class="Bound">c</a><a id="473" class="Symbol">)</a>
  <a id="477" href="Chapter2.Exercises.html#477" class="Function">ε</a> <a id="479" class="Symbol">=</a> <a id="481" href="Chapter1.Book.html#4002" class="InductiveConstructor">refl</a>
  <a id="488" href="Chapter2.Exercises.html#488" class="Function">η</a> <a id="490" class="Symbol">=</a> <a id="492" href="Chapter1.Book.html#4002" class="InductiveConstructor">refl</a>

<a id="498" class="Comment">-- Exercise 2.17 iii)</a>
<a id="520" class="Comment">-- Σ-≃-fst is on Chapter6, as it is easier to prove it with more theorems</a>
<a id="Σ-≃-snd"></a><a id="594" href="Chapter2.Exercises.html#594" class="Function">Σ-≃-snd</a> <a id="602" class="Symbol">:</a> <a id="604" class="Symbol">{</a><a id="605" href="Chapter2.Exercises.html#605" class="Bound">A</a> <a id="607" class="Symbol">:</a> <a id="609" href="Chapter1.Book.html#345" class="Function">𝒰</a> <a id="611" href="Chapter1.Book.html#328" class="Generalizable">𝒾</a><a id="612" class="Symbol">}</a> <a id="614" class="Symbol">{</a><a id="615" href="Chapter2.Exercises.html#615" class="Bound">P</a> <a id="617" class="Symbol">:</a> <a id="619" href="Chapter2.Exercises.html#605" class="Bound">A</a> <a id="621" class="Symbol">→</a> <a id="623" href="Chapter1.Book.html#345" class="Function">𝒰</a> <a id="625" href="Chapter1.Book.html#330" class="Generalizable">𝒿</a><a id="626" class="Symbol">}</a> <a id="628" class="Symbol">{</a><a id="629" href="Chapter2.Exercises.html#629" class="Bound">Q</a> <a id="631" class="Symbol">:</a> <a id="633" href="Chapter2.Exercises.html#605" class="Bound">A</a> <a id="635" class="Symbol">→</a> <a id="637" href="Chapter1.Book.html#345" class="Function">𝒰</a> <a id="639" href="Chapter1.Book.html#332" class="Generalizable">𝓀</a><a id="640" class="Symbol">}</a>
        <a id="650" class="Symbol">→</a> <a id="652" class="Symbol">((</a><a id="654" href="Chapter2.Exercises.html#654" class="Bound">x</a> <a id="656" class="Symbol">:</a> <a id="658" href="Chapter2.Exercises.html#605" class="Bound">A</a><a id="659" class="Symbol">)</a> <a id="661" class="Symbol">→</a> <a id="663" href="Chapter2.Exercises.html#615" class="Bound">P</a> <a id="665" href="Chapter2.Exercises.html#654" class="Bound">x</a> <a id="667" href="Chapter2.Book.html#8761" class="Function Operator">≃</a> <a id="669" href="Chapter2.Exercises.html#629" class="Bound">Q</a> <a id="671" href="Chapter2.Exercises.html#654" class="Bound">x</a><a id="672" class="Symbol">)</a>
        <a id="682" class="Symbol">→</a> <a id="684" href="Chapter1.Book.html#1550" class="Function">-Σ</a> <a id="687" href="Chapter2.Exercises.html#605" class="Bound">A</a> <a id="689" href="Chapter2.Exercises.html#615" class="Bound">P</a> <a id="691" href="Chapter2.Book.html#8761" class="Function Operator">≃</a> <a id="693" href="Chapter1.Book.html#1550" class="Function">-Σ</a> <a id="696" href="Chapter2.Exercises.html#605" class="Bound">A</a> <a id="698" href="Chapter2.Exercises.html#629" class="Bound">Q</a>
<a id="700" href="Chapter2.Exercises.html#594" class="Function">Σ-≃-snd</a> <a id="708" href="Chapter2.Exercises.html#708" class="Bound">f</a> <a id="710" class="Symbol">=</a> <a id="712" href="Chapter2.Exercises.html#759" class="Function">map</a> <a id="716" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="718" href="Chapter2.Book.html#8273" class="Function">invs⇒equivs</a> <a id="730" href="Chapter2.Exercises.html#759" class="Function">map</a> <a id="734" class="Symbol">(</a><a id="735" href="Chapter2.Exercises.html#799" class="Function">map⁻¹</a> <a id="741" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="743" href="Chapter2.Exercises.html#841" class="Function">ε</a> <a id="745" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="747" href="Chapter2.Exercises.html#889" class="Function">η</a><a id="748" class="Symbol">)</a>
 <a id="751" class="Keyword">where</a>
  <a id="759" href="Chapter2.Exercises.html#759" class="Function">map</a> <a id="763" class="Symbol">=</a> <a id="765" class="Symbol">λ</a> <a id="767" class="Symbol">(</a><a id="768" href="Chapter2.Exercises.html#768" class="Bound">x</a> <a id="770" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="772" href="Chapter2.Exercises.html#772" class="Bound">px</a><a id="774" class="Symbol">)</a> <a id="776" class="Symbol">→</a> <a id="778" class="Symbol">(</a><a id="779" href="Chapter2.Exercises.html#768" class="Bound">x</a> <a id="781" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="783" href="Chapter2.Book.html#8878" class="Function">≃-→</a> <a id="787" class="Symbol">(</a><a id="788" href="Chapter2.Exercises.html#708" class="Bound">f</a> <a id="790" href="Chapter2.Exercises.html#768" class="Bound">x</a><a id="791" class="Symbol">)</a> <a id="793" href="Chapter2.Exercises.html#772" class="Bound">px</a><a id="795" class="Symbol">)</a>
  <a id="799" href="Chapter2.Exercises.html#799" class="Function">map⁻¹</a> <a id="805" class="Symbol">=</a> <a id="807" class="Symbol">λ</a> <a id="809" class="Symbol">(</a><a id="810" href="Chapter2.Exercises.html#810" class="Bound">x</a> <a id="812" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="814" href="Chapter2.Exercises.html#814" class="Bound">px</a><a id="816" class="Symbol">)</a> <a id="818" class="Symbol">→</a> <a id="820" class="Symbol">(</a><a id="821" href="Chapter2.Exercises.html#810" class="Bound">x</a> <a id="823" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="825" href="Chapter2.Book.html#8941" class="Function">≃-←</a> <a id="829" class="Symbol">(</a><a id="830" href="Chapter2.Exercises.html#708" class="Bound">f</a> <a id="832" href="Chapter2.Exercises.html#810" class="Bound">x</a><a id="833" class="Symbol">)</a> <a id="835" href="Chapter2.Exercises.html#814" class="Bound">px</a><a id="837" class="Symbol">)</a>
  <a id="841" href="Chapter2.Exercises.html#841" class="Function">ε</a> <a id="843" class="Symbol">=</a> <a id="845" class="Symbol">λ</a> <a id="847" class="Symbol">(</a><a id="848" href="Chapter2.Exercises.html#848" class="Bound">x</a> <a id="850" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="852" href="Chapter2.Exercises.html#852" class="Bound">px</a><a id="854" class="Symbol">)</a> <a id="856" class="Symbol">→</a> <a id="858" href="Chapter2.Book.html#13404" class="Function">pair⁼</a><a id="863" class="Symbol">(</a><a id="864" href="Chapter1.Book.html#4002" class="InductiveConstructor">refl</a> <a id="869" href="Chapter2.Exercises.html#848" class="Bound">x</a> <a id="871" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="873" href="Chapter2.Book.html#9046" class="Function">≃-ε</a> <a id="877" class="Symbol">(</a><a id="878" href="Chapter2.Exercises.html#708" class="Bound">f</a> <a id="880" href="Chapter2.Exercises.html#848" class="Bound">x</a><a id="881" class="Symbol">)</a> <a id="883" href="Chapter2.Exercises.html#852" class="Bound">px</a><a id="885" class="Symbol">)</a>
  <a id="889" href="Chapter2.Exercises.html#889" class="Function">η</a> <a id="891" class="Symbol">=</a> <a id="893" class="Symbol">λ</a> <a id="895" class="Symbol">(</a><a id="896" href="Chapter2.Exercises.html#896" class="Bound">x</a> <a id="898" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="900" href="Chapter2.Exercises.html#900" class="Bound">px</a><a id="902" class="Symbol">)</a> <a id="904" class="Symbol">→</a> <a id="906" href="Chapter2.Book.html#13404" class="Function">pair⁼</a><a id="911" class="Symbol">(</a><a id="912" href="Chapter1.Book.html#4002" class="InductiveConstructor">refl</a> <a id="917" href="Chapter2.Exercises.html#896" class="Bound">x</a> <a id="919" href="Chapter1.Book.html#1501" class="InductiveConstructor Operator">,</a> <a id="921" href="Chapter2.Book.html#9196" class="Function">≃-η</a> <a id="925" class="Symbol">(</a><a id="926" href="Chapter2.Exercises.html#708" class="Bound">f</a> <a id="928" href="Chapter2.Exercises.html#896" class="Bound">x</a><a id="929" class="Symbol">)</a> <a id="931" href="Chapter2.Exercises.html#900" class="Bound">px</a><a id="933" class="Symbol">)</a>
</pre>