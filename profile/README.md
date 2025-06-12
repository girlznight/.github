# 📝 YellowMemo.
### [Branch 전략 - 꼭 보기!!!](https://github.com/girlznight/Project-GirzDay-react-repo/blob/main/README.md)

[UIシナリオ / UI Scenario](https://www.figma.com/design/bHP3cXgSJ24emyrV1yNXRT/Untitled?node-id=0-1&t=94VpRgeA6CHY3eCb-1)

### コミットルール / Commit Rule : [Gitmoji](https://gitmoji.dev/)

```bash
npm i -g gitmoji-cli     
gitmoji -c
```

---

<img alt="Image" src="https://github.com/user-attachments/assets/d91eb918-1423-4869-a666-5c2476aa4e3e" width="200" height="200"/>

  
## 🔗 リポジトリ / Repositories

- [PROJECT REPO](https://github.com/girlznight/Project-GirzDay-react-repo)
- [기타 관련 레포 / Others](#)

---

## 📖 プロジェクト紹介 / Project Overview

**日本語**  
小さくても、大切なアイデア。
YellowMemo. プロジェクトは、ある日、机の上に置かれた一枚の黄色い付箋から始まりました。
ふと浮かんだ考えや、通り過ぎるアイデアを、どこかに残して共有したいと思ったのです。
このアプリは、複雑な機能ではなく、「記録すること」そのものに焦点を当てて作られました。
ReactとJSON Serverで開発されており、
メモを書いて、直して、消す——そのすべての流れが、自然でシンプルになるように設計されています。
データ構造はシンプルですが、
その中には、「考えを大切にしたい」という小さな哲学が込められています。

**English**  
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
- **ドラッグ&ドロップ対応のメモボード / Drag & Drop Memo Board**
テキストボックスや画像を自由にドラッグして配置可能。位置情報はリアルタイムで保存され、UI上で直感的に操作できる。
Textboxes and images can be freely dragged and positioned; their locations are updated in real time for intuitive interaction.

- **インタラクティブなサイドバー / Interactive Sidebar**
サイドバーはトグルボタンで表示・非表示を切り替え可能。プロフィール画像、フィルター付きの投稿リスト、スクロール対応。
The sidebar can be toggled on and off, features a profile image, filterable post list, and supports scrolling.

- **レスポンシブ＆モダンUIデザイン / Responsive & Modern UI Design**
Tailwind CSSを活用し、どのデバイスでも美しく見えるレイアウトとアニメーションを実現。ホバーやフェード、スクロール時のエフェクトも実装。
Uses Tailwind CSS for beautiful layouts and animations across all devices, including hover, fade, and scroll-triggered effects.

- **プロフィール画像の編集機能 / Editable Profile Image**
プロフィール画像はアップロード・変更が可能で、未設定時はデフォルト画像を表示。
Users can upload and edit their profile image; a default image is shown if none is set.

- **スクロールアニメーション付きアバウトセクション / About Section with Scroll Animation**
「About this project」セクションはスクロール時にフェードインし、ページの下部に自然に表示される。
The "About this project" section fades in with a scroll animation, appearing naturally at the bottom of the page.

- **アクセシブルなカスタムボタン / Accessible Custom Buttons**
すべての主要操作はカスタムボタンで統一されており、アクセシビリティと一貫したUXを実現。
All main actions use custom buttons for consistent UX and accessibility.

- **リアルタイムな投稿リストの更新 / Real-time Post List Updates**
投稿が追加・更新・削除されるとサイドバーのリストが自動的に最新状態に更新される。
The sidebar post list updates automatically in real time when posts are added, updated, or deleted.

---

## 🛠 技術スタック / Tech Stack

- **フロントエンド / Frontend**: React.js 
- **バックエンド / Backend**: JSON server

---

## 📚 主なAPI・DB設計 / Main API & DB Design

- **エンドポイント分類 / Endpoint Categories**  


<details>
<summary>エンドポイント分類 / Endpoint Categories</summary>

- GET /user/:id      // 사용자 정보 조회 (Get user info)
- PATCH /user/:id     // 프로필 이미지 등 사용자 정보 수정 (Update user profile)
- GET /post        // 전체 포스트 목록 조회 (Get all posts)
- GET /post/:id      // 특정 포스트 조회 (Get post by id)
- POST /post        // 포스트 생성 (Create new post)
- GET /textbox?postId=:id // 특정 포스트의 텍스트박스 목록 조회 (Get textboxes for a post)
- POST /textbox      // 텍스트박스 생성 (Create textbox)
- GET /image?postId=:id  // 특정 포스트의 이미지 목록 조회 (Get images for a post)
- POST /image       // 이미지 생성 (Create image)
- GET /auth        // 인증 정보 조회 (Get auth info)
- POST /auth       // 인증 정보 생성 (Create auth info)
そのほか必要に応じてエンドポイント追加 (Other endpoints as needed)
</details>
  
- **DBテーブル / Database Structure**:  
<details>
<summary>user</summary>

| Field     | Type   | Description                   |
|-----------|--------|-------------------------------|
| id        | number | Unique user ID                |
| loginId   | string | Login ID                      |
| profile   | string | Profile image (Base64 format) |

</details>

<details>
<summary>auth</summary>

| Field     | Type   | Description                       |
|-----------|--------|-----------------------------------|
| id        | number | Unique auth ID                    |
| password  | string | Password                          |
| userId    | number | Linked user ID (foreign key)      |

</details>

<details>
<summary>post</summary>

| Field     | Type   | Description                       |
|-----------|--------|-----------------------------------|
| id        | number | Unique post ID                    |
| userId    | number | Author's user ID (foreign key)    |

</details>

<details>
<summary>textbox</summary>

| Field     | Type   | Description                       |
|-----------|--------|-----------------------------------|
| id        | number | Unique textbox ID                 |
| x         | number | X position                        |
| y         | number | Y position                        |
| postId    | number | Parent post ID (foreign key)      |
| content   | string | Text content                      |

</details>

<details>
<summary>postit</summary>

| Field     | Type   | Description                       |
|-----------|--------|-----------------------------------|
| id        | number | Unique post-it ID                 |
| x         | number | X position                        |
| y         | number | Y position                        |
| z         | number | Z-index (stacking order)          |
| postId    | number | Parent post ID (foreign key)      |
| content   | string | Memo content                      |
| userId    | number | Author's user ID (foreign key)    |

</details>

<details>
<summary>image</summary>

| Field     | Type   | Description                       |
|-----------|--------|-----------------------------------|
| id        | number | Unique image ID                   |
| x         | number | X position                        |
| y         | number | Y position                        |
| z         | number | Z-index (stacking order)          |
| postId    | number | Parent post ID (foreign key)      |
| src       | string | Image source (Base64 format)      |
| userId    | number | Uploader's user ID (foreign key)  |

</details>

---

## 🎯 プロジェクトの目的 / Project Purpose

**日本語:**  
YellowMemoプロジェクトは、日常の中でふと浮かぶアイデアや気付きを、簡単に記録・共有できる空間を提供することを目的としています。複雑な機能ではなく、ユーザーが直感的にメモを書き、編集し、削除できる自然な体験を重視します。シンプルなデータ構造と使いやすいインターフェースを通じて、ユーザーのあらゆる考えを大切にし、個人の創造性と協力をサポートするサービスを目指しています。

**English:**  
The purpose of the YellowMemo project is to provide a simple and intuitive platform where users can easily record and share ideas that arise in their daily lives. Rather than focusing on complex features, the project emphasizes a natural and seamless user experience for writing, editing, and deleting memos. By adopting a minimal data structure and user-friendly interface, YellowMemo aims to value every user’s thoughts and support both individual creativity and collaborative efforts

---

## 📎 参考 / References

- [API仕様書 / API Specification](https://www.notion.so/207052ad29dc8064b4b6c6c46db69f2d?source=copy_link)
- [DBテーブル設計 / DB Table Design](https://www.notion.so/DB-207052ad29dc80b1b986f21b748014ad?source=copy_link)
- [UIシナリオ / UI Scenario](https://www.figma.com/design/bHP3cXgSJ24emyrV1yNXRT/Untitled?node-id=0-1&t=94VpRgeA6CHY3eCb-1)

---
