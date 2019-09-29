<div class="instructions--content--1JI0g"><div class="instructions--title--3vSDk" data-purpose="exercise-title">Person</div><div class="instructions--description--2Qd_w"><p>Write a class with the name <strong>Person. </strong>The class needs <strong>three fields (instance variables)</strong> with the names <strong>firstName, lastName </strong>of type<strong> String </strong>and <strong>age </strong>of type <strong>int</strong>.</p><p>Write the following <strong>methods</strong> (instance methods):</p><ul><li><p>Method named <strong>getFirstName</strong> <strong>without</strong> <strong>any parameters</strong>, it needs to <strong>return</strong> the value of the <strong>firstName</strong> field.</p></li><li><p>Method named <strong>getLastName</strong> <strong>without</strong> <strong>any parameters</strong>, it needs to <strong>return</strong> the value of the <strong>lastName</strong> field.</p></li><li><p>Method named <strong>getAge</strong> <strong>without</strong> <strong>any parameters</strong>, it needs to <strong>return</strong> the value of the <strong>age </strong>field.</p></li><li><p>Method named <strong>setFirstName</strong> <strong>with one parameter of type String</strong>, it needs to <strong>set the value</strong> of the <strong>firstName</strong> field.</p></li><li><p>Method named <strong>setLastName with one parameter of type String</strong>, it needs to <strong>set the value</strong> of the <strong>lastName </strong>field.</p></li><li><p>Method named <strong>setAge with one parameter of type int</strong>, it needs to <strong>set the value</strong> of the <strong>age </strong>field. If the <strong>parameter </strong>is <strong>less than 0 or greater than 100,</strong> it needs to set the <strong>age</strong> field value to <strong>0</strong>.</p></li><li><p>Method named <strong>isTeen without any parameters, </strong>it needs to <strong>return true</strong> if the value of the <strong>age</strong> field is <strong>greater than 12 and less than 20, </strong>otherwise, <strong>return false</strong>.</p></li><li><p>Method named <strong>getFullName without any parameters, </strong>it needs to return the full name of the person.</p><ul><li><p>In case both <strong>firstName</strong> and <strong>lastName </strong>fields are empty, Strings <strong>return an empty String</strong>.</p></li><li><p>In case <strong>lastName</strong> is an empty String, <strong>return firstName.</strong></p></li><li><p>In case <strong>firstName</strong> is an empty String, <strong>return lastName.</strong></p></li></ul></li></ul><p>To check if s String is empty, use the method <strong>isEmpty</strong> from the <strong>String</strong> class. For example,<strong>firstName.isEmpty()</strong> returns true if the String is empty or in other words, when the String does not contain any characters.</p><p><br></p><p><strong>TEST EXAMPLE</strong></p><p><strong>TEST CODE:</strong></p><div class="ud-component--base-components--code-block" ng-non-bindable=""><div><pre class="prettyprint linenums prettyprinted" role="presentation" style=""><ol class="linenums"><li class="L0"><span class="typ">Person</span><span class="pln"> person&nbsp;</span><span class="pun">=</span><span class="pln">&nbsp;</span><span class="kwd">new</span><span class="pln">&nbsp;</span><span class="typ">Person</span><span class="pun">();</span></li><li class="L1"><span class="pln">person</span><span class="pun">.</span><span class="pln">setFirstName</span><span class="pun">(</span><span class="str">""</span><span class="pun">);</span><span class="pln">&nbsp;&nbsp;&nbsp;</span><span class="com">// firstName is set to empty string</span></li><li class="L2"><span class="pln">person</span><span class="pun">.</span><span class="pln">setLastName</span><span class="pun">(</span><span class="str">""</span><span class="pun">);</span><span class="pln">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="com">// lastName is set to empty string</span></li><li class="L3"><span class="pln">person</span><span class="pun">.</span><span class="pln">setAge</span><span class="pun">(</span><span class="lit">10</span><span class="pun">);</span></li><li class="L4"><span class="typ">System</span><span class="pun">.</span><span class="kwd">out</span><span class="pun">.</span><span class="pln">println</span><span class="pun">(</span><span class="str">"fullName= "</span><span class="pln">&nbsp;</span><span class="pun">+</span><span class="pln"> person</span><span class="pun">.</span><span class="pln">getFullName</span><span class="pun">());</span></li><li class="L5"><span class="typ">System</span><span class="pun">.</span><span class="kwd">out</span><span class="pun">.</span><span class="pln">println</span><span class="pun">(</span><span class="str">"teen= "</span><span class="pln">&nbsp;</span><span class="pun">+</span><span class="pln"> person</span><span class="pun">.</span><span class="pln">isTeen</span><span class="pun">());</span></li><li class="L6"><span class="pln">person</span><span class="pun">.</span><span class="pln">setFirstName</span><span class="pun">(</span><span class="str">"John"</span><span class="pun">);</span><span class="pln">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="com">// firstName is set to John</span></li><li class="L7"><span class="pln">person</span><span class="pun">.</span><span class="pln">setAge</span><span class="pun">(</span><span class="lit">18</span><span class="pun">);</span></li><li class="L8"><span class="typ">System</span><span class="pun">.</span><span class="kwd">out</span><span class="pun">.</span><span class="pln">println</span><span class="pun">(</span><span class="str">"fullName= "</span><span class="pln">&nbsp;</span><span class="pun">+</span><span class="pln"> person</span><span class="pun">.</span><span class="pln">getFullName</span><span class="pun">());</span></li><li class="L9"><span class="typ">System</span><span class="pun">.</span><span class="kwd">out</span><span class="pun">.</span><span class="pln">println</span><span class="pun">(</span><span class="str">"teen= "</span><span class="pln">&nbsp;</span><span class="pun">+</span><span class="pln"> person</span><span class="pun">.</span><span class="pln">isTeen</span><span class="pun">());</span></li><li class="L0"><span class="pln">person</span><span class="pun">.</span><span class="pln">setLastName</span><span class="pun">(</span><span class="str">"Smith"</span><span class="pun">);</span><span class="pln">&nbsp;&nbsp;&nbsp;&nbsp;</span><span class="com">// lastName is set to Smith</span></li><li class="L1"><span class="typ">System</span><span class="pun">.</span><span class="kwd">out</span><span class="pun">.</span><span class="pln">println</span><span class="pun">(</span><span class="str">"fullName= "</span><span class="pln">&nbsp;</span><span class="pun">+</span><span class="pln"> person</span><span class="pun">.</span><span class="pln">getFullName</span><span class="pun">());</span></li></ol></pre></div></div><p><strong>OUTPUT</strong></p><div class="ud-component--base-components--code-block" ng-non-bindable=""><div><pre class="prettyprint linenums prettyprinted" role="presentation" style=""><ol class="linenums"><li class="L0"><span class="pln">fullName</span><span class="pun">=</span></li><li class="L1"><span class="pln">teen</span><span class="pun">=</span><span class="pln">&nbsp;</span><span class="kwd">false</span></li><li class="L2"><span class="pln">fullName</span><span class="pun">=</span><span class="pln">&nbsp;</span><span class="typ">John</span></li><li class="L3"><span class="pln">teen</span><span class="pun">=</span><span class="pln">&nbsp;</span><span class="kwd">true</span></li><li class="L4"><span class="pln">fullName</span><span class="pun">=</span><span class="pln">&nbsp;</span><span class="typ">John</span><span class="pln"> </span><span class="typ">Smith</span></li></ol></pre></div></div><p><br></p><p><strong>NOTE:</strong> All <strong>​</strong>methods should be defined as<strong> public NOT public static</strong>.</p><p><strong>NOTE:</strong> In total, you have to write <strong>8 methods</strong>.</p><p><strong>NOTE:</strong> Do not add the <strong>main </strong>method to the solution code.</p></div></div><div class="instructions--drag-handle--ocDGT"></div>