---
layout: page
title: 회원가입
permalink: /register/
---

<div class="auth-form">
  <form id="register-form">
    <div class="form-group">
      <label for="name">이름</label>
      <input type="text" id="name" name="name" required>
    </div>
    <div class="form-group">
      <label for="email">이메일</label>
      <input type="email" id="email" name="email" required>
    </div>
    <div class="form-group">
      <label for="password">비밀번호</label>
      <input type="password" id="password" name="password" required>
    </div>
    <div class="form-group">
      <label for="password-confirm">비밀번호 확인</label>
      <input type="password" id="password-confirm" name="password-confirm" required>
    </div>
    <div class="form-actions">
      <button type="submit">가입하기</button>
    </div>
    <p class="form-help">
      이미 계정이 있으신가요? <a href="{{ '/login/' | relative_url }}">로그인</a>
    </p>
  </form>
</div>

<script>
document.getElementById('register-form').addEventListener('submit', function(e) {
  e.preventDefault();
  
  // 비밀번호 확인
  const password = document.getElementById('password').value;
  const passwordConfirm = document.getElementById('password-confirm').value;
  
  if (password !== passwordConfirm) {
    alert('비밀번호가 일치하지 않습니다.');
    return;
  }
  
  // 여기에 회원가입 로직을 구현합니다.
  // 예: Disqus나 다른 인증 제공자를 통한 회원가입
  
  alert('회원가입 기능은 현재 구현 중입니다. 곧 사용 가능해질 예정입니다.');
});
</script> 