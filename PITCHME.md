---
### Python駿河 勉強会 #4  LT

#### iPad ProでPythonの開発環境を作る

2019/08/24 @Bivi藤枝

---

### お前誰よは割愛

Twitter @hrs_sano645 です

---

### iPad ProでPython開発環境？

---

### Why?
---

### iPad Proは軽くてパワフル

軽さは正義

---

### 以上

---

### 作り方

---

### pythonistaがあればよくない？

---

### まあそうなんだけど
---

### ディストリビューションに縛られず

---

### デスクトップやサーバー環境と同じがいい

---
### 今のところこうしてる

- 適当なサーバー+VPN
- エディタ
- sshクライアント
- Gitクライアント

---

## サーバーは自前で用意

- 適当なサーバー
  - 事務所のVMマシンサーバーにLinux入れてる
- クラウドでもよし(AWS, MS, Google)
- Raspberry Pi（ラズパイ）を家に置いて接続とか

VPNはお好みで良いかと

自分はOpenVPN使ってます

---

### サーバーへ接続はどうする？
---

### SSHクライアント

- Prompt2
- Termius
- **Shelly**

---

### どうやってPython書くの？

- ssh接続できるなら Vim/Emacsでも
- iPadのエディタ
    - [‎Textastic](https://apps.apple.com/jp/app/textastic-code-editor-8/id1049254261) 
      - おすすめ（エディタ+SSH/SFTPクライアント）
    - [‎GoCoEdit](https://apps.apple.com/jp/app/gocoedit-code-text-editor/id869346854)
    - ほかにも色々

コード補完は難しい（スニペットなら手段はありそう）

デバッグはSSH経由になる（テスト駆動、リンターを通すとか）

---

### コードの管理はどうする？

（そもそもそんなにコード書けるのかは？さておき）

---

### コードの管理

Githubにあるコードをローカルでみたい時に便利

- [‎Working Copy](https://apps.apple.com/jp/app/working-copy/id896694807)
- [‎GoCoEdit](https://apps.apple.com/jp/app/gocoedit-code-text-editor/id869346854)

---
#### 参考例:iPadのみで今日のスライドを作ってた様子

呟いた様子

https://twitter.com/hrs_sano645/status/1164127492333981696

---

### おまけのおまけ

---

### ちなみにAndroidだと

---

### Termuxというアプリ

[Termux - Google Play のアプリ](https://play.google.com/store/apps/details?id=com.termux&hl=ja)

- サンドボックス+コンテナ技術で、AndroidでLinuxが動く！！！
- 1台で開発環境ができる。羨ましい！！

---

### もっといいもの

[Google Chromebooks](https://www.google.com/intl/ja_jp/chromebook/features/)

- chromeOS+Linux+Androidアプリ動く（ざっというとそういうもの）
- 北米方面ではよく使われているらしい
- 日本でも手に入るけどスペックが微妙
- Pixelbookが日本に来たら欲しかった！😂

---

### 今後考えてること

---

### リモート環境だとネット環境心配...

---

### 小型のマシンを持てば良いのでは？

- SBCをもつ！つまりラズパイあたり
- ラズパイ4来たら勝つのでは？（メモリ最大4GB積むのでかなり動くはず）
    - ラズパイ
    - ssh/リモートデスクトップで見れる
- モバイルバッテリーで動けばなおさら良いけど。。

---

### でもラズパイとモニターとキーボードがあればよくね

 -> iPad Proいらなくね？

---

### そこはロマンですし

---

### まとめ

---

### iPad ProでPython開発は頑張ればできる

ただネットがないと辛い

---
### iOS13だとよりデスクトップ環境らしくなるのでさらに期待！

- WEB IDEが動く可能性あり, VS CodeベースのVisual Studio Online
    - [マイクロソフトがVisual Studio Onlineプレビュー版を発表 | TechCrunch Japan](https://jp.techcrunch.com/2019/05/07/2019-05-06-microsoft-launches-visual-studio-online-an-online-code-editor/)
    - VS CodeをWEBで動かすプロジェクトは他にもある
      - [Coder](https://coder.com/)

- AWS Cloud 9も動くといいな 

