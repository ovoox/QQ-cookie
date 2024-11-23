# QQ-cookie
<div style="position: relative;">
  <pre id="copyText" style="background-color: #f5f5f5; padding: 10px; border: 1px solid #ccc;">
这是一个示例文本，你可以点击右上角的按钮复制这段文字。
  </pre>
  <button onclick="copyToClipboard()" style="position: absolute; top: 5px; right: 5px;">复制</button>
</div>

<script>
function copyToClipboard() {
  const text = document.getElementById('copyText').innerText;
  navigator.clipboard.writeText(text).then(() => {
    alert('文本已复制到剪贴板');
  }).catch(err => {
    console.error('复制失败', err);
  });
}
</script>
