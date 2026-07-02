---
layout: page
title: 产品列表
---

<script>
(function() {
  var lang = (navigator.language || navigator.userLanguage || '').toLowerCase();
  if (lang.startsWith('en') && !location.hash) {
    window.location.replace('{{ "/en/" | relative_url }}');
  }
})();
</script>

<div class="product-grid">

<a href="{{ "/StoreSnap/" | relative_url }}" class="product-card">
  <div class="product-card-inner">
    <img src="{{ "/StoreSnap/images/icon.png" | relative_url }}" alt="" class="product-icon">
    <div>
      <h2 class="product-name">StoreSnap</h2>
      <p class="product-desc">App Store 截图生成工具。拖拽、选择、导出，三步搞定，把时间留给代码。</p>
    </div>
  </div>
</a>

<a href="{{ "/DoodleLanguage/" | relative_url }}" class="product-card">
  <div class="product-card-inner">
    <img src="{{ "/DoodleLanguage/images/icon.png" | relative_url }}" alt="" class="product-icon">
    <div>
      <h2 class="product-name">DoodleLanguage</h2>
      <p class="product-desc">画涂鸦学外语。画一只猫，记住 "cat"。专为儿童和视觉型学习者设计。</p>
    </div>
  </div>
</a>

<a href="{{ "/DeepBalance/" | relative_url }}" class="product-card">
  <div class="product-card-inner">
    <img src="{{ "/DeepBalance/images/icon.png" | relative_url }}" alt="" class="product-icon">
    <div>
      <h2 class="product-name">DeepBalance+</h2>
      <p class="product-desc">DeepSeek 余额查看工具。菜单栏速览余额，Widget 实时更新，打开即用。</p>
    </div>
  </div>
</a>

</div>

<div class="site-footer-bar">
  <a href="{{ site.url }}{{ site.baseurl }}">{{ site.url }}{{ site.baseurl }}</a>
</div>
