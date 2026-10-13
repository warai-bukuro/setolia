[English](README-en.md)

# SETOLIA

OBS Studio 用セットリストプラグイン

## 主な機能

- 配信時間に同期したタイムスタンプ
- 曲番号の自動採番
- リアルタイム時計表示
- [歌詞検索サイト](https://utaten.com)へのショートカットボタン
- 設定済みブラウザソース追加ボタン
- カスタムテンプレートに対応
- Stream Deck からの操作に対応

## インストール方法

Windows、MacOS、Linux 用のバイナリは、[リリース](https://github.com/Yagami-Huki/setolia/releases)ページで入手可能です。

また、[Booth](https://logicbox.booth.pm/items/7541386) にて最新の Windows 用のインストーラーを入手可能です。

### ポータブル版 OBS へのインストール

`portable` フォルダに OBS を展開した上で `scripts/deploy_to_portable.ps1` を実行してください。

## ビルド方法

要件: Visual Studio 2026（C++ デスクトップ開発ワークロード）、CMake 3.28 以降

依存関係は CMake の configure 時に自動ダウンロードされます。

```powershell
cmake --preset windows-x64
cmake --build --preset windows-x64
cmake --install build_x64
```

`cmake --install` のデフォルトのインストール先は `C:\ProgramData\obs-studio\plugins\setolia` です。

macOS / Linux の場合は `CMakePresets.json` の `macos` / `ubuntu-x86_64` プリセットを使用してください。

## 使用方法

[Booth](https://logicbox.booth.pm/items/7541386) にてユーザーマニュアルを公開しているため、こちらをご参照ください。

## ライセンスと謝辞

このソフトウェアは、GPL-3.0 ライセンスのもとで公開されています。

このプロジェクトは、[OBS Project](https://github.com/obsproject) によって作成された [obs-plugintemplate](https://github.com/obsproject/obs-plugintemplate) を使用して開発されました。

また、このソフトウェアに付属する標準のテンプレートは、MIT ライセンスのもとで公開されています。
