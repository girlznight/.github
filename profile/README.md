# 📝 YellowMemo.
> 🗒️ YellowMemo is a sticky-note style idea board for your floating ideas.

### [Branch 전략 - 꼭 보기!!!](https://github.com/girlznight/Project-GirzDay-react-repo/blob/main/README.md)

<img alt="Image" src="https://github.com/user-attachments/assets/d91eb918-1423-4869-a666-5c2476aa4e3e" width="200" height="200"/>

  
## 🔗 リポジトリ / Repositories

- [PROJECT REPO](https://github.com/girlznight/Project-GirzDay-react-repo)

---

## 📖 プロジェクト紹介 / Project Overview

**🇯🇵**  
小さくても、大切なアイデア。
YellowMemo. プロジェクトは、ある日、机の上に置かれた一枚の黄色い付箋から始まりました。
ふと浮かんだ考えや、通り過ぎるアイデアを、どこかに残して共有したいと思ったのです。
このアプリは、複雑な機能ではなく、「記録すること」そのものに焦点を当てて作られました。
ReactとJSON Serverで開発されており、
メモを書いて、直して、消す——そのすべての流れが、自然でシンプルになるように設計されています。
データ構造はシンプルですが、
その中には、「考えを大切にしたい」という小さな哲学が込められています。

**🇺🇸**  
Small, but essential ideas.
The YellowMemo. project began one day with a single yellow sticky note left on a desk.
We wanted to keep and share thoughts that popped into our minds—ideas that come and go in an instant.
This app was created not to focus on complex features, but to simply honor the act of recording ideas.
Built with React and a JSON server,
It’s designed so that writing, editing, and deleting a memo flows naturally and simply.
Though the data structure is minimal,
It carries a quiet philosophy: to respect every thought, no matter how small.

---

## 🌟 主な機能 / Key Features
**ドラッグ&ドロップ対応のメモボード / Drag & Drop Memo Board**  
`🇯🇵 テキストボックスや画像を自由にドラッグして配置可能。位置情報はリアルタイムで保存され、UI上で直感的に操作できる。
🇺🇸 Textboxes and images can be freely dragged and positioned; their locations are updated in real time for intuitive interaction.
`

**インタラクティブなサイドバー / Interactive Sidebar**

🇯🇵 サイドバーはトグルボタンで表示・非表示を切り替え可能。プロフィール画像、フィルター付きの投稿リスト、スクロール対応。
🇺🇸 The sidebar can be toggled on and off, features a profile image, filterable post list, and supports scrolling.

**レスポンシブ＆モダンUIデザイン / Responsive & Modern UI Design**

🇯🇵 Tailwind CSSを活用し、どのデバイスでも美しく見えるレイアウトとアニメーションを実現。ホバーやフェード、スクロール時のエフェクトも実装。
🇺🇸 Uses Tailwind CSS for beautiful layouts and animations across all devices, including hover, fade, and scroll-triggered effects.

**プロフィール画像の編集機能 / Editable Profile Image**

🇯🇵 プロフィール画像はアップロード・変更が可能で、未設定時はデフォルト画像を表示。
🇺🇸 Users can upload and edit their profile image; a default image is shown if none is set.

**スクロールアニメーション付きアバウトセクション / About Section with Scroll Animation**

🇯🇵 「About this project」セクションはスクロール時にフェードインし、ページの下部に自然に表示される。
The "About this project" section fades in with a scroll animation, appearing naturally at the bottom of the page.

**アクセシブルなカスタムボタン / Accessible Custom Buttons**

🇯🇵 すべての主要操作はカスタムボタンで統一されており、アクセシビリティと一貫したUXを実現。
🇺🇸 All main actions use custom buttons for consistent UX and accessibility.

**リアルタイムな投稿リストの更新 / Real-time Post List Updates**

🇯🇵 投稿が追加・更新・削除されるとサイドバーのリストが自動的に最新状態に更新される。
🇺🇸 The sidebar post list updates automatically in real time when posts are added, updated, or deleted.

---

## 🛠 技術スタック / Tech Stack

- **Frontend**: React.js, Tailwind CSS  
- **Backend**: JSON Server  
- **Others**: Base64 Encoding 

---

## 📚 API & Database Design

- All API endpoints follow RESTful principles.
- Data managed with JSON Server (local mock DB).
- Key tables: `user`, `post`, `textbox`, `image`, `postit`, `auth`

📎 [Detailed API Docs](https://www.notion.so/207052ad29dc8064b4b6c6c46db69f2d)  
📎 [DB Structure Notion](https://www.notion.so/DB-207052ad29dc80b1b986f21b748014ad)
---
## 🎯 Purpose

**🇯🇵**
YellowMemo は、思いついたその瞬間のアイデアを素早く記録し、ビジュアルに整理するための空間を目指して開発されました。
単なるメモアプリではなく、「アイデアを育てる庭」をコンセプトにしています。🌱

**🇺🇸**
YellowMemo was developed as a space to quickly capture and visually organize fleeting ideas.
It’s more than a memo app — it’s an idea garden. 🌱


---

## 📎 参考 / References

- [API仕様書 / API Specification](https://www.notion.so/207052ad29dc8064b4b6c6c46db69f2d?source=copy_link)
- [DBテーブル設計 / DB Table Design](https://www.notion.so/DB-207052ad29dc80b1b986f21b748014ad?source=copy_link)
- [UIシナリオ / UI Scenario](https://www.figma.com/design/bHP3cXgSJ24emyrV1yNXRT/Untitled?node-id=0-1&t=94VpRgeA6CHY3eCb-1)

---

