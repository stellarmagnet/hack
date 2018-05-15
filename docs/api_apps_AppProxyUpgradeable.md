---
id: apps_AppProxyUpgradeable
title: AppProxyUpgradeable
---

<div class="contract-doc"><div class="contract"><h2 class="contract-header"><span class="contract-kind">contract</span> AppProxyUpgradeable</h2><p class="base-contracts"><span>is</span> <a href="apps_AppProxyBase.html">AppProxyBase</a></p><div class="source">Source: <a href="https://github.com/aragon/aragonOS//blob/v3.1.4/contracts/apps/AppProxyUpgradeable.sol" target="_blank">apps/AppProxyUpgradeable.sol</a></div></div><div class="index"><h2>Index</h2><ul><li><a href="apps_AppProxyUpgradeable.html#AppProxyUpgradeable">AppProxyUpgradeable</a></li><li><a href="apps_AppProxyUpgradeable.html#implementation">implementation</a></li><li><a href="apps_AppProxyUpgradeable.html#proxyType">proxyType</a></li></ul></div><div class="reference"><h2>Reference</h2><div class="functions"><h3>Functions</h3><ul><li><div class="item function"><span id="AppProxyUpgradeable" class="anchor-marker"></span><h4 class="name">AppProxyUpgradeable</h4><div class="body"><code class="signature">function <strong>AppProxyUpgradeable</strong><span>(IKernel _kernel, bytes32 _appId, bytes _initializePayload) </span><span>public </span></code><hr/><div class="description"><p>Initialize AppProxyUpgradeable (makes it an upgradeable Aragon app).</p></div><dl><dt><span class="label-modifiers">Modifiers:</span></dt><dd></dd><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_kernel</code> - Reference to organization kernel for the app</div><div><code>_appId</code> - Identifier for app</div><div><code>_initializePayload</code> - Payload for call to be made after setup to initialize</div></dd></dl></div></div></li><li><div class="item function"><span id="implementation" class="anchor-marker"></span><h4 class="name">implementation</h4><div class="body"><code class="signature">function <strong>implementation</strong><span>() </span><span>public </span><span>view </span><span>returns  (address) </span></code><hr/><div class="description"><p>ERC897, the address the proxy would delegate calls to.</p></div><dl><dt><span class="label-return">Returns:</span></dt><dd>address</dd></dl></div></div></li><li><div class="item function"><span id="proxyType" class="anchor-marker"></span><h4 class="name">proxyType</h4><div class="body"><code class="signature">function <strong>proxyType</strong><span>() </span><span>public </span><span>pure </span><span>returns  (uint256) </span></code><hr/><div class="description"><p>ERC897, whether it is a forwarding (1) or an upgradeable (2) proxy.</p></div><dl><dt><span class="label-return">Returns:</span></dt><dd>uint256</dd></dl></div></div></li></ul></div></div></div>