---
id: evmscript_executors_DelegateScript
title: DelegateScript
---

<div class="contract-doc"><div class="contract"><h2 class="contract-header"><span class="contract-kind">contract</span> DelegateScript</h2><p class="base-contracts"><span>is</span> <a href="evmscript_IEVMScriptExecutor.html">IEVMScriptExecutor</a></p><div class="source">Source: <a href="https://github.com/aragon/aragonOS//blob/v3.1.4/contracts/evmscript/executors/DelegateScript.sol" target="_blank">evmscript/executors/DelegateScript.sol</a></div></div><div class="index"><h2>Index</h2><ul><li><a href="evmscript_executors_DelegateScript.html#defaultInput">defaultInput</a></li><li><a href="evmscript_executors_DelegateScript.html#delegate">delegate</a></li><li><a href="evmscript_executors_DelegateScript.html#execScript">execScript</a></li><li><a href="evmscript_executors_DelegateScript.html#isContract">isContract</a></li><li><a href="evmscript_executors_DelegateScript.html#returnedData">returnedData</a></li></ul></div><div class="reference"><h2>Reference</h2><div class="functions"><h3>Functions</h3><ul><li><div class="item function"><span id="defaultInput" class="anchor-marker"></span><h4 class="name">defaultInput</h4><div class="body"><code class="signature">function <strong>defaultInput</strong><span>() </span><span>internal </span><span>pure </span><span>returns  (bytes) </span></code><hr/><dl><dt><span class="label-return">Returns:</span></dt><dd>bytes</dd></dl></div></div></li><li><div class="item function"><span id="delegate" class="anchor-marker"></span><h4 class="name">delegate</h4><div class="body"><code class="signature">function <strong>delegate</strong><span>(address _addr, bytes _input) </span><span>internal </span><span>returns  (bytes) </span></code><hr/><div class="description"><p>Delegatecall to contract with input data.</p></div><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_addr</code> - address</div><div><code>_input</code> - bytes</div></dd><dt><span class="label-return">Returns:</span></dt><dd>bytes</dd></dl></div></div></li><li><div class="item function"><span id="execScript" class="anchor-marker"></span><h4 class="name">execScript</h4><div class="body"><code class="signature">function <strong>execScript</strong><span>(bytes _script, bytes _input, address[] _blacklist) </span><span>external </span><span>returns  (bytes) </span></code><hr/><div class="description"><p>Executes script by delegatecall into a contract.</p></div><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_script</code> - [ specId (uint32) ][ contract address (20 bytes) ]</div><div><code>_input</code> - ABI encoded call to be made to contract (if empty executes default exec() function)</div><div><code>_blacklist</code> - If any address is passed, will revert.</div></dd><dt><span class="label-return">Returns:</span></dt><dd>Call return data</dd></dl></div></div></li><li><div class="item function"><span id="isContract" class="anchor-marker"></span><h4 class="name">isContract</h4><div class="body"><code class="signature">function <strong>isContract</strong><span>(address _target) </span><span>internal </span><span>view </span><span>returns  (bool) </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_target</code> - address</div></dd><dt><span class="label-return">Returns:</span></dt><dd>bool</dd></dl></div></div></li><li><div class="item function"><span id="returnedData" class="anchor-marker"></span><h4 class="name">returnedData</h4><div class="body"><code class="signature">function <strong>returnedData</strong><span>() </span><span>internal </span><span>pure </span><span>returns  (bytes) </span></code><hr/><div class="description"><p>Copies and returns last&#x27;s call data.</p></div><dl><dt><span class="label-return">Returns:</span></dt><dd>bytes</dd></dl></div></div></li></ul></div></div></div>