<div class="instructions--content--1JI0g"><div class="instructions--title--3vSDk" data-purpose="exercise-title">Sum Calculator</div><div class="instructions--description--2Qd_w"><p>Write a class with the name <strong>SimpleCalculator. </strong>The class needs <strong>two fields (instance variables)</strong> with names <strong>firstNumber</strong> and <strong>secondNumber </strong>both of type <strong>double</strong>.</p><p>Write the following methods (instance methods):</p><ul><li><p>Method named <strong>getFirstNumber</strong> <strong>without</strong> <strong>any parameters</strong>, it needs to <strong>return</strong> the value of <strong>firstNumber</strong> field.</p></li><li><p>Method named <strong>getSecondNumber</strong> <strong>without</strong> <strong>any parameters</strong>, it needs to <strong>return</strong> the value of <strong>secondNumber</strong> field.</p></li><li><p>Method named <strong>setFirstNumber</strong> <strong>with one parameter of type double</strong>, it needs to <strong>set the value</strong> of the <strong>firstNumber</strong> field.</p></li><li><p>Method named <strong>setSecondNumber with one parameter of type double</strong>, it needs to <strong>set the value</strong> of the <strong>secondNumber</strong>field.</p></li><li><p>Method named <strong>getAdditionResult without any parameters, </strong>it needs to <strong>return </strong>the result of <strong>adding</strong> the field values of <strong>firstNumber</strong> and <strong>secondNumber</strong>.</p></li><li><p>Method named <strong>getSubtractionResult without any parameters</strong>, it needs to <strong>return</strong> the result of <strong>subtracting</strong> the field values of <strong>secondNumber</strong> from the <strong>firstNumber</strong>.</p></li><li><p>Method named <strong>getMultiplicationResult without any parameters</strong>, it needs to <strong>return</strong> the result of <strong>multiplying </strong>the field values of <strong>firstNumber </strong>and <strong>secondNumber.</strong></p></li><li><p>Method named <strong>getDivisionResult</strong> <strong>without any parameters</strong> it needs to <strong>return</strong> the result of <strong>dividing</strong> the field values of <strong>firstNumber</strong> by the <strong>secondNumber. </strong>In case the value of <strong>secondNumber</strong> is <strong>0 then return 0</strong>.</p></li></ul><p><br></p><p><strong>TEST EXAMPLE</strong></p><p><strong>TEST CODE:</strong></p><div class="ud-component--base-components--code-block" ng-non-bindable=""><div><pre class="prettyprint linenums prettyprinted" role="presentation" style=""><ol class="linenums"><li class="L0"><span class="typ">SimpleCalculator</span><span class="pln"> calculator&nbsp;</span><span class="pun">=</span><span class="pln">&nbsp;</span><span class="kwd">new</span><span class="pln">&nbsp;</span><span class="typ">SimpleCalculator</span><span class="pun">();</span></li><li class="L1"><span class="pln">calculator</span><span class="pun">.</span><span class="pln">setFirstNumber</span><span class="pun">(</span><span class="lit">5.0</span><span class="pun">);</span></li><li class="L2"><span class="pln">calculator</span><span class="pun">.</span><span class="pln">setSecondNumber</span><span class="pun">(</span><span class="lit">4</span><span class="pun">);</span></li><li class="L3"><span class="typ">System</span><span class="pun">.</span><span class="kwd">out</span><span class="pun">.</span><span class="pln">println</span><span class="pun">(</span><span class="str">"add= "</span><span class="pln">&nbsp;</span><span class="pun">+</span><span class="pln"> calculator</span><span class="pun">.</span><span class="pln">getAdditionResult</span><span class="pun">());</span></li><li class="L4"><span class="typ">System</span><span class="pun">.</span><span class="kwd">out</span><span class="pun">.</span><span class="pln">println</span><span class="pun">(</span><span class="str">"subtract= "</span><span class="pln">&nbsp;</span><span class="pun">+</span><span class="pln"> calculator</span><span class="pun">.</span><span class="pln">getSubtractionResult</span><span class="pun">());</span></li><li class="L5"><span class="pln">calculator</span><span class="pun">.</span><span class="pln">setFirstNumber</span><span class="pun">(</span><span class="lit">5.25</span><span class="pun">);</span></li><li class="L6"><span class="pln">calculator</span><span class="pun">.</span><span class="pln">setSecondNumber</span><span class="pun">(</span><span class="lit">0</span><span class="pun">);</span></li><li class="L7"><span class="typ">System</span><span class="pun">.</span><span class="kwd">out</span><span class="pun">.</span><span class="pln">println</span><span class="pun">(</span><span class="str">"multiply= "</span><span class="pln">&nbsp;</span><span class="pun">+</span><span class="pln"> calculator</span><span class="pun">.</span><span class="pln">getMultiplicationResult</span><span class="pun">());</span></li><li class="L8"><span class="typ">System</span><span class="pun">.</span><span class="kwd">out</span><span class="pun">.</span><span class="pln">println</span><span class="pun">(</span><span class="str">"divide= "</span><span class="pln">&nbsp;</span><span class="pun">+</span><span class="pln"> calculator</span><span class="pun">.</span><span class="pln">getDivisionResult</span><span class="pun">());</span></li></ol></pre></div></div><p><strong>OUTPUT</strong></p><div class="ud-component--base-components--code-block" ng-non-bindable=""><div><pre class="prettyprint linenums prettyprinted" role="presentation" style=""><ol class="linenums"><li class="L0"><span class="pln">add</span><span class="pun">=</span><span class="pln">&nbsp;</span><span class="lit">9.0</span></li><li class="L1"><span class="pln">subtract</span><span class="pun">=</span><span class="pln">&nbsp;</span><span class="lit">1.0</span></li><li class="L2"><span class="pln">multiply</span><span class="pun">=</span><span class="pln">&nbsp;</span><span class="lit">0.0</span></li><li class="L3"><span class="pln">divide</span><span class="pun">=</span><span class="pln">&nbsp;</span><span class="lit">0.0</span></li></ol></pre></div></div><p><strong>TIPS:</strong></p><ul><li><p><code><strong>add= 9.0</strong></code><strong> </strong>is printed because 5.0 + 4 is 9.0</p></li><li><p><code><strong>subtract= 1.0</strong></code><strong> </strong>is printed because 5.0 - 4 is 1.0</p></li><li><p><code><strong>multiply= 0.0</strong></code><strong> </strong>is printed because 5.25 * 0 is 0.0</p></li><li><p><code><strong>divide= 0.0</strong></code><strong> </strong>is printed because <strong>secondNumber is set to 0</strong></p></li></ul><p><br></p><p><strong>NOTE:</strong> All <strong>​</strong>methods should be defined as<strong> public NOT public static</strong>.</p><p><strong>NOTE:</strong> In total, you have to write <strong>8 methods</strong>.</p><p><strong>NOTE:</strong> Do not add the <strong>main </strong>method to the solution code.</p></div></div><div class="instructions--drag-handle--ocDGT"></div>