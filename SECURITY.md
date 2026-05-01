# セキュリティポリシー / Security Policy

## 脆弱性の報告 / Reporting a Vulnerability

国民民主党 奈良県総支部連合会 候補者公募サイトのセキュリティ脆弱性を発見された場合は、
以下の連絡先まで責任あるご開示をお願いいたします。

If you discover a security vulnerability, please disclose it responsibly via:

- **Email**: info@new-kokumin-nara.jp
- **件名 / Subject**: `[Security] {脆弱性の概要}`

### 報告に含めるべき情報 / Please Include

1. 影響を受けるページ・機能 / Affected page or feature
2. 脆弱性の説明 / Description
3. 再現手順 / Steps to reproduce
4. 想定される影響 / Potential impact
5. (任意) 推奨される修正方法 / (Optional) Suggested fix

### 対応について / Response

- 受領後、48時間以内に初回返信いたします
- 重大な脆弱性は最優先で対応します
- 公表前に報告者と協議し、対応方針を共有します

## 対応範囲 / Scope

### In Scope
- https://new-kokumin-nara.jp/ 配下のすべてのページ
- 応募フォーム (FormSubmit.co 経由)
- リポジトリ: https://github.com/tkaminobiz-art/kokuminnaraV2

### Out of Scope
- スパム・ブルートフォース・DoS
- ソーシャルエンジニアリング
- 物理的アクセス
- 第三者サービスの脆弱性 (FormSubmit.co、GitHub Pages、Google Fonts 等の本体)

## 対応中の対策 / Implemented Mitigations

- HTTPS強制 (GitHub Pages デフォルト)
- Content Security Policy (CSP) 実装
- X-Content-Type-Options / Permissions-Policy 設定
- フォーム: Honeypot + reCAPTCHA (FormSubmit) + ファイル検証 (PDF magic bytes)
- 個人情報の最小化収集

## 謝意 / Acknowledgments

責任あるご開示をいただいた方には、希望に応じてサイトに謝辞を掲載させていただきます。
