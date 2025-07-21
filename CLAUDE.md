作るもの：タスク管理アプリ「My Daily Tasks」
シンプルで実用的なToDoリストアプリケーションを作成します。日常のタスクを管理し、完了状況を追跡できます。
主な機能

タスクの追加・編集・削除
タスクの完了/未完了の切り替え
カテゴリー別のタスク分類（仕事、プライベート、勉強など）
タスクの優先度設定（高・中・低）
完了タスクのフィルタリング表示
ローカルストレージへのデータ保存

使用技術
コア技術

Vite 5.x - 高速な開発環境とビルドツール
React 18.x - UIライブラリ
TypeScript 5.x - 型安全な開発
MUI 5.x - マテリアルデザインコンポーネント

追加ライブラリ

@mui/icons-material - アイコンセット
@emotion/react, @emotion/styled - スタイリング
uuid - タスクIDの生成用

プロジェクト概要
画面構成

ヘッダー - アプリタイトルとダークモード切り替え
タスク入力フォーム - 新規タスク追加
フィルターバー - カテゴリーと状態でフィルタリング
タスクリスト - タスク一覧表示
統計情報 - 完了率などの表示

データ構造（TypeScript型定義）
typescriptinterface Task {
  id: string;
  title: string;
  description?: string;
  category: 'work' | 'personal' | 'study';
  priority: 'high' | 'medium' | 'low';
  completed: boolean;
  createdAt: Date;
  completedAt?: Date;
}
