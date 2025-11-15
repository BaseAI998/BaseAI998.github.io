---
layout: none
title: 关于我
permalink: /about
---

<!DOCTYPE html>
<html lang="zh-CN">
  <head>
    <meta charset="UTF-8" />
    <title>关于我 - {{ site.title }}</title>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link rel="stylesheet" href="/assets/css/style.css" />
  </head>
  <body>
    <header class="site-header">
      <div class="container header-inner">
        <div class="logo-area">
          <div class="logo-dot"></div>
          <div>
            <div class="site-title">{{ site.title }}</div>
            <div class="site-subtitle">{{ site.description }}</div>
          </div>
        </div>
        <nav class="nav">
          {% for item in site.nav %}
          <a href="{{ item.url }}">{{ item.name }}</a>
          {% endfor %}
        </nav>
      </div>
    </header>

    <main class="container main page">
      <h1>关于我</h1>
      <p>这里写一点自我介绍，比如：</p>
      <ul>
        <li>是谁、在做什么</li>
        <li>感兴趣的方向（算法竞赛、AI、Web3、产品、设计等）</li>
        <li>这个博客准备写些什么</li>
      </ul>
    </main>

    <footer class="site-footer">
      <div class="container footer-inner">
        <span>© {{ "now" | date: "%Y" }} {{ site.author }}</span>
        <span>由 GitHub Pages & Jekyll 驱动</span>
      </div>
    </footer>
  </body>
</html>
