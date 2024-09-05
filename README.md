# スキーマのサンプル

## 概要

JSONやXMLのスキーマ情報を設定するサンプルです。

## ファイル種別

### JSON

- Json Schemaを使ってスキーマを定義します
- スキーマファイルは`schema/sample.schema.json`です
- ファイル内で指定するときには`$schema`で指定します
- VS Codeで一括で指定する場合、`settings.json`に`json.schemas`を指定します

### YAML

- Json Schemaを使ってスキーマを定義します
- スキーマファイルは`schema/sample.schema.json`です
- ファイル内で指定するときには`# yaml-language-server: $schema=～`で指定します
- VS Codeで一括で指定する場合、`settings.json`に`yaml.schemas`を指定します
- `yaml.schemas`の指定にはVS拡張`YAML Language Support by Red Hat`をインストールする必要があります

### XML

- XML Schemaを使ってスキーマを定義します
- スキーマファイルは`schema/sample.sample.xsd`です
- ファイル内で指定するときには`xsi:noNamespaceSchemaLocation="～"`で指定します（`xmlns:xsi=～`も必要です）
- VS Codeで一括で指定する場合、`settings.json`に`xml.fileAssociations`を指定します
- `xml.fileAssociations`の指定にはVS拡張`XML Language Support by Red Hat`をインストールする必要があります
- パスの指定時に先頭を`**/～`ではなく`/hoge/～`とすると何故か指定が効きません
