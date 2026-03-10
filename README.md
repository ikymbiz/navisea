# navisea

## 概要・説明 / Overview & Description

**[JP]**
NaviSea（ナビシー）は、東京ディズニーシーでの1日を最高に楽しむための「パーソナルパークコンシェルジュ」ウェブアプリケーションです。
現在の待ち時間、あなたの現在地、好みのプレイスタイル（絶叫、写真映え、のんびり等）、乗りたいアトラクションを選択するだけで、AIコンシェルジュが移動がスムーズで効率的なあなただけの特別ルートを自動生成します。単なるルート案内にとどまらず、ディズニーフリークならではの「豆知識」「隠れスポット」「ショー・パレードの攻略ガイド」などを交えた可愛らしいアドバイスを提供してくれます。

**[EN]**
NaviSea is a "Personal Park Concierge" web application designed to help you make the most of your day at Tokyo DisneySea.
By simply selecting your desired attractions, preferred play style (thrill-seeking, photogenic, relaxing, etc.), and factoring in real-time wait times and your current GPS location, the AI concierge automatically generates a highly optimized and personalized route. Beyond basic navigation, it provides charming advice filled with Disney geek trivia, hidden spots, and parade-viewing tips.

---

## スクリーンショット / Screenshots

![NaviSea Screenshot 1](https://via.placeholder.com/600x400?text=NaviSea+Top+Screen)
![NaviSea Screenshot 2](https://via.placeholder.com/600x400?text=NaviSea+Generated+Plan)

*(プレースホルダーです。実際のスクリーンショット画像に差し替えてください / Please replace with actual screenshots)*

---

## 主な機能一覧 / Key Features

**[JP]**
- **リアルタイム待ち時間の同期**: 外部APIからアトラクションの最新の待ち時間と運営状況を取得して一覧表示。
- **パーソナライズされたルート生成**: 現在地（Geolocation API）、出発日時、選択したアトラクションから最適なスケジュールをAIが計算。
- **プレイスタイルの選択**: 「おまかせ」「絶叫全力！」「写真映え✨」「のんびり☕️」から好みに合わせたプランニングが可能。
- **フリーメモ機能**: 「ランチ予約済み」「特定のキャラクターに会いたい」などの詳細な要望をプランに反映。
- **マニアックなパークアドバイス**: 移動中の豆知識、待ち時間の活用方法、写真スポットなどをAIコンシェルジュが提案。

**[EN]**
- **Real-Time Wait Time Sync**: Fetches and displays the latest attraction wait times and operational status from an external API.
- **Personalized Route Generation**: Calculates the optimal schedule using AI based on your current location (Geolocation API), start time, and selected attractions.
- **Play Style Selection**: Choose from "Balanced", "Thrill", "Photogenic", or "Chill" to tailor the plan to your mood.
- **Custom Notes**: Add specific requests like "Lunch booked" or "Want to meet Duffy" to integrate into your plan.
- **Geeky Park Advice**: The AI concierge suggests trivia, hidden photo spots, and ways to kill time while waiting in line.

---

## 使用技術・ライブラリ / Technologies & Libraries

**[JP]**
- **フロントエンド**: HTML5, CSS3 (Vanilla), JavaScript (Vanilla)
- **API・通信**: Fetch API
- **位置情報**: Geolocation API (現在地の取得)
- **バックエンド・AI連携**: Cloudflare Workers (LLMへのプロンプト送信・JSONレスポンス解析)
- **データソース**: GitHub Pages上にホストされた外部JSONデータ (待ち時間取得)

**[EN]**
- **Frontend**: HTML5, CSS3 (Vanilla), JavaScript (Vanilla)
- **API/Network**: Fetch API
- **Location**: Geolocation API (for getting current user coordinates)
- **Backend/AI Integration**: Cloudflare Workers (for handling LLM prompts and parsing JSON responses)
- **Data Source**: External JSON hosted on GitHub Pages (for fetching wait times)

---

## セットアップ・使い方 / Setup & Usage

**[JP]**
1. このプロジェクトの `index.html` をダウンロード、またはリポジトリをクローンします。
2. Webブラウザ（Chrome, Safari等）で `index.html` を開きます。（※現在地取得機能を使用するため、HTTPS環境またはlocalhostでの実行を推奨します）
3. **API Key (Optional)**: 必要に応じて指定のAPIキーを入力します（ローカルストレージに保存されます）。
4. **Plan Setting**: パークを回り始める日時と、好みのプレイスタイルを選択します。
5. **Select Spots & Events**: リストから行きたいアトラクションをタップして選択します（待ち時間も確認できます）。
6. **Notes**: レストランの予約や特別な希望があればテキストボックスに入力します。
7. 「**⛵ プランを作成する**」ボタンをクリックすると、位置情報が取得され、画面下部にAIコンシェルジュからの特別なルートとアドバイスが表示されます。

**[EN]**
1. Download `index.html` or clone this repository.
2. Open `index.html` in a web browser like Chrome or Safari. (*Note: Running on HTTPS or localhost is recommended to allow the Geolocation API to work properly.*)
3. **API Key (Optional)**: Enter the required API key if needed (it will be saved in your local storage).
4. **Plan Setting**: Select your start time and preferred play style persona.
5. **Select Spots & Events**: Tap on the attractions you want to visit from the list (current wait times are displayed).
6. **Notes**: Enter any specific requests, such as restaurant reservations, into the text box.
7. Click the "**⛵ プランを作成する (Create Plan)**" button. The app will fetch your location and display a special route and tips from the AI concierge at the bottom of the screen.

---

## ライセンス / License

**[JP]**
このプロジェクトは MIT ライセンスの下で公開されています。詳細については、LICENSE ファイルを参照してください。（※必要に応じて変更してください）

**[EN]**
This project is licensed under the MIT License. See the LICENSE file for details. (*Modify as needed*)