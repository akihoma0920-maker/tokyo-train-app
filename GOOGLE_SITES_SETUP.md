# 🚀 Google Sitesで使用する方法

## 📌 推奨方法：外部ホスティング + 埋め込み

Google Sitesには直接HTMLファイルをアップロードできないため、以下の方法を使用します。

---

## ✅ 方法1: GitHub Pages（最も簡単・推奨）

### **ステップ1: GitHubにアップロード**

1. GitHubアカウントを作成（https://github.com）
2. 新しいリポジトリを作成
   - リポジトリ名: `tokyo-train-app`
   - Public を選択
3. 全てのファイルをアップロード：
   ```
   index.html
   css/style.css
   js/data.js
   js/main.js
   js/conversation.js
   README.md
   ```

### **ステップ2: GitHub Pagesを有効化**

1. リポジトリの「Settings」をクリック
2. 左メニューから「Pages」を選択
3. Source: 「Deploy from a branch」を選択
4. Branch: 「main」を選択、フォルダ: 「/ (root)」を選択
5. 「Save」をクリック
6. 数分後、URLが表示されます：  
   `https://あなたのユーザー名.github.io/tokyo-train-app/`

### **ステップ3: Google Sitesに埋め込む**

1. Google Sitesを開く
2. 「挿入」→「埋め込み」を選択
3. GitHub PagesのURLを入力
4. サイズを調整（推奨: 幅100%、高さ800px）
5. 「挿入」をクリック

---

## ✅ 方法2: Netlify（無料・簡単）

### **ステップ1: Netlifyにデプロイ**

1. Netlifyアカウントを作成（https://www.netlify.com/）
2. 「Add new site」→「Deploy manually」を選択
3. 全てのファイルをドラッグ＆ドロップ
4. 自動的にURLが生成されます：  
   `https://ランダム文字.netlify.app/`

### **ステップ2: Google Sitesに埋め込む**

1. Google Sitesを開く
2. 「挿入」→「埋め込み」を選択
3. NetlifyのURLを入力
4. サイズを調整
5. 「挿入」をクリック

---

## ✅ 方法3: オールインワンHTMLファイル（制限あり）

この方法は、全てのコードを1つのHTMLファイルにまとめます。

### **メリット：**
- ファイル1つだけでOK
- 外部サービス不要

### **デメリット：**
- ファイルサイズが大きい（約100KB）
- Google Sitesで直接アップロードできない
- 画像URLは外部を使用

### **手順：**

1. `tokyo-train-app-standalone.html` ファイルを作成（後述）
2. Google Driveにアップロード
3. 共有設定を「リンクを知っている全員」に変更
4. Google Sitesの「埋め込み」でGoogle DriveのプレビューURLを使用

**注意：** Google DriveのHTML表示には制限があるため、GitHub PagesまたはNetlifyを推奨します。

---

## 🎯 最も簡単な方法（ステップバイステップ）

### **GitHub Pagesを使用（初心者向け）**

#### **1. GitHubアカウント作成**
- https://github.com にアクセス
- 「Sign up」をクリック
- メールアドレス、パスワードを入力

#### **2. 新しいリポジトリ作成**
- 右上の「+」→「New repository」をクリック
- Repository name: `tokyo-train-app`
- Public を選択
- 「Create repository」をクリック

#### **3. ファイルをアップロード**
- 「uploading an existing file」をクリック
- 全てのファイルをドラッグ＆ドロップ
  - index.html
  - css/style.css
  - js/data.js
  - js/main.js
  - js/conversation.js
  - README.md
- 「Commit changes」をクリック

#### **4. GitHub Pagesを有効化**
- 「Settings」タブをクリック
- 左メニュー「Pages」をクリック
- Source: 「main」を選択
- 「Save」をクリック
- 緑色の通知に表示されるURLをコピー

#### **5. Google Sitesに埋め込む**
- Google Sites を開く
- ページを編集
- 「挿入」→「埋め込み」をクリック
- コピーしたURLを貼り付け
- 幅: 100%、高さ: 800px に設定
- 「挿入」をクリック

---

## 📱 埋め込み設定の推奨値

```html
幅: 100%
高さ: 800px ~ 1000px

または

<iframe 
  src="あなたのURL" 
  width="100%" 
  height="800" 
  frameborder="0">
</iframe>
```

---

## 🔧 トラブルシューティング

### **問題1: 画像が表示されない**
**解決策：** 画像URLが正しいか確認してください。外部URLを使用する必要があります。

### **問題2: CORSエラー**
**解決策：** GitHub PagesまたはNetlifyを使用してください。これらはCORS問題を自動的に解決します。

### **問題3: Google Sitesで埋め込みが表示されない**
**解決策：**
1. URLが `https://` で始まっているか確認
2. 埋め込みサイズを調整（高さを増やす）
3. ブラウザのキャッシュをクリア

---

## ✨ 推奨設定

### **最良の組み合わせ：**
1. **ホスティング：** GitHub Pages（無料・安定）
2. **埋め込み先：** Google Sites
3. **画像：** 外部URL（現在のままでOK）

### **この組み合わせのメリット：**
- ✅ 完全無料
- ✅ 高速・安定
- ✅ 自動SSL（https）
- ✅ 簡単な更新（GitHubで編集するだけ）
- ✅ バージョン管理
- ✅ Google Sitesと完全互換

---

## 📞 サポート

質問がある場合は、READMEファイルを確認してください。

**Made with ❤️ for Night School Students**
