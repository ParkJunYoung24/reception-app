# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# 社内受付アプリ

## 概要
タブレット（iPad）向けの社内受付キオスクアプリ。
サーバー不要・単一HTMLファイルで完結。

## 技術スタック
- バニラHTML / CSS / JavaScript のみ
- Web Audio API（来客・配達の通知音）
- localStorage（履歴保存）

## 機能要件
- 来客ボタン・配達ボタンを大きく表示
- ボタン押下で通知音を鳴らす
- 営業時間（9:00〜18:30）の表示・時間外グレーアウト
- 履歴画面はPINコード（1234）で保護
- 履歴は日付・種別で確認できる

## iPad対応
- タッチ操作最適化
- 全画面表示（100dvh）
- 誤タップ・誤スクロール防止

## 制約
- 外部ライブラリ・CDN禁止
- ビルド不要・index.html 1ファイルで完結