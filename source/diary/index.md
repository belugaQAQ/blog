---
title: 文章归档
date: 2025-12-21
layout: diary
---

<div class="diary-page">
  <div class="diary-title">
    <h1>文章归档</h1>
    <p>共找到 <%= site.posts.length %> 篇文章</p>
  </div>
  
  <div class="diary-list">
    <% site.posts.sort('date', -1).each(function(post) { %>
      <div class="diary-item">
        <div class="diary-date">
          <%- date(post.date, 'YYYY-MM-DD') %>
        </div>
        <div class="diary-title">
          <a href="<%- url_for(post.path) %>"><%- post.title %></a>
        </div>
      </div>
    <% }); %>
  </div>
</div>