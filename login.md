---
layout: page
title: 로그인
permalink: /login/
---

<div class="auth-form">
  <form id="login-form">
    <div class="form-group">
      <label for="email">이메일</label>
      <input type="email" id="email" name="email" required>
    </div>
    <div class="form-group">
      <label for="password">비밀번호</label>
      <input type="password" id="password" name="password" required>
    </div>
    <div class="form-actions">
      <button type="submit">로그인</button>
    </div>
    <p class="form-help">
      계정이 없으신가요? <a href="{{ '/register/' | relative_url }}">회원가입</a>
    </p>
  </form>
</div>

<script>
document.getElementById('login-form').addEventListener('submit', function(e) {
  e.preventDefault();
  
  // 여기에 로그인 로직을 구현합니다.
  // 예: Disqus나 다른 인증 제공자를 통한 로그인
  
  alert('로그인 기능은 현재 구현 중입니다. 곧 사용 가능해질 예정입니다.');
});
</script> 