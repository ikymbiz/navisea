# navisea
夢の航海プラン 〜あなただけのスマートなパーク周遊アプリ〜
Your Smart Voyage Plan - Personalized Theme Park Routing App

## 概要 / Overview

**[🇯🇵 日本語]**
NaviSea (ParkHack) は、東京ディズニーシーを効率的かつ自分らしく楽しむためのスマート周遊プラン作成Webアプリケーションです。
リアルタイムの待ち時間データ、過去の混雑傾向、ユーザーの現在地、そして「絶叫好き」「のんびり」「子連れ」などのペルソナ設定を組み合わせ、AIがあなたにぴったりの最適な周遊ルートを提案します。可愛らしく洗練されたUIで、パークでの一日をハックします。

**[🇬🇧 English]**
NaviSea (ParkHack) is a smart itinerary-building web application designed to help you enjoy Tokyo DisneySea efficiently and in your own style. 
By combining real-time wait times, historical crowd trends, user geolocation, and personalized preferences (e.g., Thrill-seeker, Chill, Kids-friendly), an AI generates the optimal route tailored just for you. The app features a cute and sophisticated UI to "hack" your day at the park.

---

## 主な機能一覧 / Key Features

**[🇯🇵 日本語]**
- 🕒 **リアルタイム待ち時間表示**: 外部APIと連携し、現在のアトラクション待ち時間を一覧表示。
- 📊 **混雑予測トレンドグラフ**: Chart.jsを使用し、過去のデータ傾向と現在の待ち時間から今後の混雑状況を予測・可視化。
- 📍 **現在地の反映**: Geolocation APIを利用し、パーク内の現在地情報から最適な移動距離・ルートを考慮。
- 🤖 **AI最適ルート生成**: 選択したアトラクション、ペルソナ設定、自由入力メモ（「ランチ予約済み」など）を基に、AIが時間ごとの詳細なプランとアドバイスを作成。
- 🔍 **スマート検索＆フィルター**: 「雨天OK」「絶叫」「キッズ」などのタグ絞り込みや、待ち時間順のソート機能。

**[🇬🇧 English]**
- 🕒 **Real-time Wait Times**: Fetches and displays current attraction wait times via an external JSON API.
- 📊 **Crowd Trend Graph**: Uses Chart.js to visualize predicted wait times based on historical data and current conditions.
- 📍 **Geolocation Integration**: Utilizes the Geolocation API to factor in your current location within the park for optimal routing and minimal walking.
- 🤖 **AI-Powered Route Generation**: Creates a detailed, time-based itinerary and practical tips using AI, based on selected attractions, persona, and custom notes (e.g., "Lunch booked at 1 PM").
- 🔍 **Smart Search & Filters**: Filter attractions by tags like "Rain OK", "Thrill", "Kids", or sort them by wait times.

---

## 使用技術・ライブラリ / Technologies & Libraries

- **Frontend**: HTML5, CSS3, Vanilla JavaScript (No heavy frameworks used)
- **Data Visualization**: [Chart.js](https://www.chartjs.org/) (Loaded via CDN)
- **APIs & Services**:
  - Browser Geolocation API
  - Custom JSON API (Real-time wait times data synchronization)
  - Cloudflare Workers / LLM Integration (Backend API for AI prompt processing and JSON response generation)

---

## セットアップ・使い方 / Setup & Usage

**[🇯🇵 日本語]**
1. **セットアップ**: 
   特別なビルド環境は不要です。提供された単一の `index.html` ファイルをブラウザで直接開くか、任意のWebサーバー（GitHub Pages、Vercelなど）にデプロイするだけで動作します。
2. **使い方**:
   - 画面上部で「開始時間」と「ペルソナ（おまかせ、絶叫全力！、子連れで安心など）」を選択します。
   - パーク内にいる場合は `📍 パーク内にいる場合は現在地を取得` ボタンを押して位置情報を許可します。
   - リストから行きたいアトラクションをタップして選択します。（各リストの `📊` ボタンを押すと混雑傾向グラフが確認できます）
   - 必要に応じてメモ欄に要望や困りごとを入力し、`⛵ 最適なプランを作成する` ボタンを押します。
   - AIが計算した、あなただけの航海プランが表示されます！

**[🇬🇧 English]**
1. **Setup**: 
   No complex build tools or package managers are required. Simply open the provided `index.html` file in any modern web browser or host it on a web server (e.g., GitHub Pages, Vercel).
2. **Usage**:
   - Select your starting time and persona (e.g., Balanced, Thrill-seeker, Kids-friendly) at the top of the screen.
   - Click the `📍 Get Location` button if you are currently inside the park to allow GPS tracking.
   - Tap on the attractions you want to visit from the list. (Click the `📊` icon to view the crowd trend prediction graph).
   - Add any specific requests in the text area (e.g., "Don't want to walk too much"), then click the `⛵ Generate Optimal Plan` button.
   - Enjoy your AI-generated, customized smart route and tips!

---

## スクリーンショット / Screenshots

![App Home Screen](https://via.placeholder.com/800x400/f8dbd5/5a4a42?text=NaviSea+Home+Screen+Placeholder)
*アトラクション選択・フィルター画面 / Attraction Selection & Filter Screen*

![Trend Graph](https://via.placeholder.com/800x400/b9d8eb/5a4a42?text=NaviSea+Trend+Graph+Placeholder)
*混雑予測トレンドグラフ / Crowd Trend Graph Modal*

![Generated Plan](https://via.placeholder.com/800x400/d4a373/ffffff?text=NaviSea+AI+Generated+Plan+Placeholder)
*AI生成による航海プラン / AI-Generated Voyage Plan*

---

## ライセンス / License

**[🇯🇵 日本語]**
このプロジェクトは [MIT License](LICENSE) の下で公開されています。
※ **免責事項**: 本アプリケーションは個人的な学習および目的で作られた非公式のファンプロジェクトであり、東京ディズニーリゾート公式、株式会社オリエンタルランドとは一切関係ありません。

**[🇬🇧 English]**
This project is licensed under the [MIT License](LICENSE).
*Disclaimer: This is an unofficial fan project created for educational and personal purposes. It is in no way affiliated with, authorized, or endorsed by the official Tokyo Disney Resort or Oriental Land Co., Ltd.*