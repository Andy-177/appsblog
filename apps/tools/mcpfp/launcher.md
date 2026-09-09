<style>
  /* 1. 去掉内容区的所有内边距 */
  .markdown-section {
    padding: 0 !important;
    margin: 0 !important;
    max-width: 100% !important;
  }
  
  /* 2. 去掉文章内容的顶部间距 */
  .markdown-section > :first-child {
    margin-top: 0 !important;
  }
  
  /* 3. 让 iframe 从内容区最顶部开始 */
  .markdown-section iframe {
    display: block;
    width: 100%;
    height: calc(100vh); /* 40px 是顶部导航栏高度，可调 */
    border: none;
    margin: 0;
    padding: 0;
    vertical-align: top; /* 去掉 inline 元素底部空隙 */
  }
  
  /* 4. 整个内容容器顶部对齐 */
  .content {
    padding-top: 0 !important;
  }
  
  /* 5. 如果页面本身有 body 间距也去掉 */
  body {
    margin: 0;
  }
</style>
<style>
  /* 让侧边栏的切换按钮在鼠标移开时隐藏 */
  .sidebar-toggle-button {
    opacity: 0;
    transition: opacity 0.3s ease; /* 加个淡入淡出效果，更柔和 */
    pointer-events: none; /* 隐藏时无法被点击，防止误触 */
  }

  /* 当鼠标悬停在按钮上时，显示它 */
  .sidebar-toggle-button:hover {
    opacity: 1;
    pointer-events: auto;
  }

  /* 当鼠标悬停在整个侧边栏区域时，也显示按钮（可选，更符合直觉） */
  .sidebar:hover .sidebar-toggle-button {
    opacity: 1;
    pointer-events: auto;
  }
  .sidebar-toggle {
    background-color: #fff0;
  }
  .github-corner {
    display: none;
  }
</style>
[mcpfp](/index.html ':include')