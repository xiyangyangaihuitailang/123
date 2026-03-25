<template>
  <div class="welcome-page">
    <header class="hero">
      <p class="tag">Hello · 你好 · Welcome</p>
      <h1>欢迎来到我们的应用</h1>
      <p class="subtitle">很高兴见到你！这是一个简洁、现代的欢迎页示例。</p>
      <div class="actions">
        <button type="button" class="btn btn-primary">开始体验</button>
        <button type="button" class="btn btn-secondary">了解更多</button>
      </div>
    </header>

    <section class="features">
      <article class="feature-card">
        <h2>快速上手</h2>
        <p>几分钟内完成配置，立即开始你的项目。</p>
      </article>
      <article class="feature-card">
        <h2>优雅界面</h2>
        <p>清爽排版与渐变背景，带来更好的视觉体验。</p>
      </article>
      <article class="feature-card">
        <h2>灵活扩展</h2>
        <p>组件化结构，方便按需扩展功能模块。</p>
      </article>
    </section>
  </div>
</template>

<script>
export default {
  name: "App",
};
</script>

<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  background: #f4f7fb;
}


.welcome-page {
  min-height: 100vh;
  padding: 48px 20px;
  background: linear-gradient(135deg, #f7f9ff 0%, #e7eeff 100%);
  color: #1f2a44;
  font-family: "PingFang SC", "Microsoft YaHei", "Helvetica Neue", Arial, sans-serif;
}

.hero {
  max-width: 760px;
  margin: 0 auto;
  text-align: center;
}

.tag {
  display: inline-block;
  margin: 0;
  padding: 6px 14px;
  border-radius: 999px;
  background: #ffffff;
  color: #4d63d3;
  font-size: 14px;
  font-weight: 600;
}

h1 {
  margin: 18px 0 12px;
  font-size: 44px;
  line-height: 1.2;
}

.subtitle {
  margin: 0 auto;
  max-width: 560px;
  font-size: 18px;
  color: #4b5b7a;
}

.actions {
  margin-top: 28px;
  display: flex;
  justify-content: center;
  gap: 14px;
  flex-wrap: wrap;
}

.btn {
  border: none;
  border-radius: 10px;
  padding: 12px 24px;
  font-size: 16px;
  font-weight: 600;
  cursor: pointer;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.btn:hover {
  transform: translateY(-1px);
}

.btn-primary {
  background: #4d63d3;
  color: #fff;
  box-shadow: 0 8px 20px rgba(77, 99, 211, 0.25);
}

.btn-secondary {
  background: #fff;
  color: #344b9a;
  border: 1px solid #cdd7f8;
}

.features {
  margin: 48px auto 0;
  max-width: 980px;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
  gap: 16px;
}

.feature-card {
  background: #fff;
  border-radius: 14px;
  padding: 20px;
  text-align: left;
  box-shadow: 0 10px 24px rgba(39, 65, 130, 0.08);
}

.feature-card h2 {
  margin: 0;
  font-size: 20px;
}

.feature-card p {
  margin: 10px 0 0;
  color: #5a6886;
  line-height: 1.6;
}
</style>
