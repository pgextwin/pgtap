# pgTAP — Windows x64 バイナリ

[English](README.md) | 日本語

[pgTAP](https://github.com/theory/pgtap)の**非公式Windows x64バイナリ**です。pgTAPはPostgreSQL内でTAP形式の単体テストを行う拡張機能です。

## ダウンロードと対応環境

[最新の公開Release](https://github.com/pgextwin/pgtap/releases/latest)からダウンロードできます。[過去のReleases](https://github.com/pgextwin/pgtap/releases)も確認できます。PostgreSQL **14〜18**向けの配布状況は[pgextwinカタログ](https://pgextwin.github.io/website/ja/)を参照してください。利用中のPostgreSQLメジャーバージョンに一致するZIPを使用します。PostgreSQL 14のコミュニティサポートは2026年11月12日までです。

## インストール

1. PostgreSQL環境のバックアップを取得し、[上流ドキュメント](https://github.com/theory/pgtap)で必要条件を確認します。
2. 既存ファイルを置き換える前にPostgreSQLを停止し、対応するZIPを展開します。
3. ZIPに含まれるlib/とshare/extension/以下のファイルを、PostgreSQLの同名ディレクトリに配置します。
4. PostgreSQLを起動し、利用するデータベースでCREATE EXTENSION pgtap;を実行します。

ReleaseのSHA256SUMS.txtでZIPを照合してください。SPDX形式のSBOM、脆弱性レポート、署名付き証明の有無もReleaseで確認できます。本番導入前に動作確認を行ってください。

## 上流プロジェクトとライセンス

使い方と制限事項は[上流のpgTAP](https://github.com/theory/pgtap)を参照してください。pgextwinは独立した非公式配布であり、上流開発元の承認を示すものではありません。ライセンスは配布物に含まれる表記に従います。
