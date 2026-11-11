# 第7回 Webエンジニアリング演習 レポート
## 学籍番号
4724219
## 2画面の見出しと本文 
    if (page === "#detail") {
    app.innerHTML = `
      <h1>詳細画面</h1>
      <p>詳細ページの内容です。</p>
    `;
  } else {
    app.innerHTML = ` 
   <h1>画面生成方式の比較</h1> 
   <p>この文章はTypeScriptから追加した。</p> 
    `;
  }
});
出力結果
　画面生成方式の比較
この文章はTypeScriptから追加した。
　詳細画面
詳細ページの内容です。
## クリック後のURLとNetworkの確認
URL https://psychic-adventure-wrqr977vq66w29xx4-3000.app.github.dev/csr/#detail
    https://psychic-adventure-wrqr977vq66w29xx4-3000.app.github.dev/csr/#compare
URLをクリックしたのちにNetworkの行に新たにHTMLの行は追加されなかったことを確認した。
## 画面を切り替える処理の要点
window.addEventListener("hashchange", () => {
    const page = location.hash; 
    console.log(page)
    console.log(location.hash)
