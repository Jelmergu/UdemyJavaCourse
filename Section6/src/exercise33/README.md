<div class="instructions--content--1JI0g"><div class="instructions--title--3vSDk" data-purpose="exercise-title">Carpet Cost Calculator</div><div class="instructions--description--2Qd_w"><p>The Carpet Company has asked you to write an application that calculates the price of carpeting for rectangular rooms. To calculate the price, you multiply the area of the floor (width times length) by the price per square meter of carpet. For example, the area of the floor that is 12 meters long and 10 meters wide is 120 square meters. To cover the floor with a carpet that costs $8 per square meter would cost $960.</p><p><strong>1. </strong>Write a class with the name <strong>Floor. </strong>The class needs <strong>two fields (instance variables)</strong> with name <strong>width </strong>and <strong>length </strong>of type<strong> double</strong>.</p><p>The class needs to have one constructor with parameters <strong>width </strong>and <strong>length </strong>of type <strong>double</strong> and it needs to initialize the fields.</p><p>In case the <strong>width </strong>parameter is <strong>less than 0</strong> it needs to set the <strong>width</strong> field value to <strong>0</strong>, in case the <strong>length</strong> parameter is<strong> less than 0</strong> it needs to set the <strong>length</strong> field value to <strong>0</strong>.</p><p>Write the following <strong>methods</strong> (instance methods):</p><ul><li><p>Method named <strong>getArea</strong> <strong>without</strong> <strong>any parameters</strong>, it needs to <strong>return</strong> the calculated area <strong>(width * length)</strong>.</p></li></ul><p><br></p><p><strong>2. </strong>Write a class with the name <strong>Carpet. </strong>The class needs <strong>one field (instance variable)</strong> with name <strong>cost </strong>of type<strong> double</strong>.</p><p>The class needs to have one constructor with parameter <strong>cost </strong>of type <strong>double</strong> and it needs to initialize the field.</p><p>In case the <strong>cost </strong>parameter is <strong>less than 0</strong> it needs to set the <strong>cost </strong>field value to <strong>0.</strong></p><p>Write the following <strong>methods</strong> (instance methods):</p><ul><li><p>Method named <strong>getCost</strong> <strong>without</strong> <strong>any parameters</strong>, it needs to <strong>return</strong> the value of <strong>cost </strong>field</p></li></ul><p><br></p><p><strong>3. </strong>Write a class with the name <strong>Calculator. </strong>The class needs <strong>two fields (instance variables)</strong> with name <strong>floor</strong> of type <strong>Floor</strong> and <strong>carpet </strong>of type<strong> Carpet</strong>.</p><p>The class needs to have one constructor with parameters <strong>floor </strong>of type <strong>Floor</strong> and <strong>carpet </strong>of type <strong>Carpet</strong> and it needs to initialize the fields.</p><p>Write the following <strong>methods</strong> (instance methods):</p><ul><li><p>Method named <strong>getTotalCost</strong> <strong>without</strong> <strong>any parameters</strong>, it needs to <strong>return</strong> the calculated total cost to cover the <strong>floor</strong> with a <strong>carpet</strong>.</p></li></ul><p><br></p><p><strong>TEST EXAMPLE</strong></p><p><strong>→ TEST CODE:</strong></p><div class="ud-component--base-components--code-block" ng-non-bindable=""><div><pre class="prettyprint linenums prettyprinted" role="presentation" style=""><ol class="linenums"><li class="L0"><span class="typ">Carpet</span><span class="pln"> carpet </span><span class="pun">=</span><span class="pln"> </span><span class="kwd">new</span><span class="pln"> </span><span class="typ">Carpet</span><span class="pun">(</span><span class="lit">3.5</span><span class="pun">);</span></li><li class="L1"><span class="typ">Floor</span><span class="pln"> floor </span><span class="pun">=</span><span class="pln"> </span><span class="kwd">new</span><span class="pln"> </span><span class="typ">Floor</span><span class="pun">(</span><span class="lit">2.75</span><span class="pun">,</span><span class="pln"> </span><span class="lit">4.0</span><span class="pun">);</span></li><li class="L2"><span class="typ">Calculator</span><span class="pln"> calculator </span><span class="pun">=</span><span class="pln"> </span><span class="kwd">new</span><span class="pln"> </span><span class="typ">Calculator</span><span class="pun">(</span><span class="pln">floor</span><span class="pun">,</span><span class="pln"> carpet</span><span class="pun">);</span></li><li class="L3"><span class="typ">System</span><span class="pun">.</span><span class="kwd">out</span><span class="pun">.</span><span class="pln">println</span><span class="pun">(</span><span class="str">"total= "</span><span class="pln"> </span><span class="pun">+</span><span class="pln"> calculator</span><span class="pun">.</span><span class="pln">getTotalCost</span><span class="pun">());</span></li><li class="L4"><span class="pln">carpet </span><span class="pun">=</span><span class="pln"> </span><span class="kwd">new</span><span class="pln"> </span><span class="typ">Carpet</span><span class="pun">(</span><span class="lit">1.5</span><span class="pun">);</span></li><li class="L5"><span class="pln">floor </span><span class="pun">=</span><span class="pln"> </span><span class="kwd">new</span><span class="pln"> </span><span class="typ">Floor</span><span class="pun">(</span><span class="lit">5.4</span><span class="pun">,</span><span class="pln"> </span><span class="lit">4.5</span><span class="pun">);</span></li><li class="L6"><span class="pln">calculator </span><span class="pun">=</span><span class="pln"> </span><span class="kwd">new</span><span class="pln"> </span><span class="typ">Calculator</span><span class="pun">(</span><span class="pln">floor</span><span class="pun">,</span><span class="pln"> carpet</span><span class="pun">);</span></li><li class="L7"><span class="typ">System</span><span class="pun">.</span><span class="kwd">out</span><span class="pun">.</span><span class="pln">println</span><span class="pun">(</span><span class="str">"total= "</span><span class="pln"> </span><span class="pun">+</span><span class="pln"> calculator</span><span class="pun">.</span><span class="pln">getTotalCost</span><span class="pun">());</span></li></ol></pre></div></div><p><strong>→ OUTPUT</strong></p><div class="ud-component--base-components--code-block" ng-non-bindable=""><div><pre class="prettyprint linenums prettyprinted" role="presentation" style=""><ol class="linenums"><li class="L0"><span class="pln">total</span><span class="pun">=</span><span class="pln"> </span><span class="lit">38.5</span></li><li class="L1"><span class="pln">total</span><span class="pun">=</span><span class="pln"> </span><span class="lit">36.45</span></li></ol></pre></div></div><p><br></p><p><strong>NOTE:</strong> All <strong>​</strong>methods should be defined as<strong> public NOT public static</strong>.</p><p><strong>NOTE:</strong> In total, you have to write<strong> 3 classes.</strong></p><p><strong>NOTE:</strong> Do not add a <strong>main </strong>method to the solution code.</p></div></div><div class="instructions--drag-handle--ocDGT"></div>