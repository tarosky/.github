# .github

Common directory for Tarosky Organization

## テンプレート

このリポジトリには、以下のテンプレートが含まれています：

- イシューテンプレート:
  - `.github/ISSUE_TEMPLATE/generic.md`
  - `.github/ISSUE_TEMPLATE/infra.md`
- プルリクエストテンプレート:
  - `.github/PULL_REQUEST_TEMPLATE/generic.md`
  - `.github/PULL_REQUEST_TEMPLATE/infra.md`

### 既存リポジトリへのテンプレート適用方法

組織の `.github` リポジトリに追加されたテンプレートは、新規に作成されるリポジトリには自動的に適用されますが、既存のリポジトリには自動的には適用されません。既存リポジトリにテンプレートを適用するには、以下の方法があります：

#### 方法1: リポジトリ固有のテンプレートを作成する

1. 対象リポジトリに `.github` ディレクトリを作成する
2. イシューテンプレートを適用する場合：
   - `.github/ISSUE_TEMPLATE` ディレクトリを作成
   - 組織の `.github` リポジトリから `issue_template.md` をコピーして配置
3. プルリクエストテンプレートを適用する場合：
   - `.github/PULL_REQUEST_TEMPLATE.md` ファイルを作成
   - 組織の `.github` リポジトリから内容をコピー

#### 方法2: 組織のテンプレートを参照する（イシューテンプレートのみ）

GitHub では、リポジトリ固有のテンプレートがない場合に組織のテンプレートを使用するオプションがあります。これを有効にするには：

1. 対象リポジトリの Settings > General に移動
2. 「Features」セクションまでスクロール
3. 「Issues」が有効になっていることを確認
4. 「Set up templates」ボタンをクリック
5. 「Add template: select」ドロップダウンから「Use organization's default community health file」を選択

これにより、リポジトリ固有のテンプレートを作成せずに、組織のデフォルトテンプレートを使用できます。

**注意**: プルリクエストテンプレートについては、現在 GitHub は組織のデフォルトテンプレートを自動的に使用するオプションを提供していません。プルリクエストテンプレートを適用するには、方法1を使用する必要があります。
