<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1, user-scalable=no">
<title>uFit 大口発注フォーム | Order Form</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Zen+Kaku+Gothic+New:wght@500;700;900&family=Noto+Sans+JP:wght@400;500;700&family=Inter:wght@500;600;700&display=swap" rel="stylesheet">
<script src="https://cdn.tailwindcss.com"></script>
<script>
  tailwind.config = {
    theme: {
      extend: {
        colors: {
          paper: '#FAF9F6',
          ink: '#16181B',
          inksoft: '#5C6066',
          line: '#E6E3DC',
          matcha: '#3D7A5E',
          matchadark: '#2C5945',
          matchasoft: '#E7F0EA',
          honey: '#C8842B',
          honeysoft: '#FBF0DE',
          danger: '#B23B3B'
        },
        fontFamily: {
          display: ['"Zen Kaku Gothic New"', '"Noto Sans JP"', 'sans-serif'],
          body: ['"Noto Sans JP"', '"Zen Kaku Gothic New"', 'sans-serif'],
          num: ['"Inter"', '"Noto Sans JP"', 'sans-serif']
        }
      }
    }
  }
</script>
<style>
  body { font-family: 'Noto Sans JP', sans-serif; background:#FAF9F6; }
  .font-display { font-family: 'Zen Kaku Gothic New', 'Noto Sans JP', sans-serif; }
  .font-num { font-family: 'Inter', 'Noto Sans JP', sans-serif; font-variant-numeric: tabular-nums; }
  input[type=number]::-webkit-outer-spin-button,
  input[type=number]::-webkit-inner-spin-button { -webkit-appearance: none; margin:0; }
  input[type=number] { -moz-appearance: textfield; }
  .accordion-panel { max-height: 0; overflow: hidden; transition: max-height 0.35s ease; }
  .accordion-panel.open { max-height: 4000px; }
  .chev { transition: transform 0.25s ease; }
  .chev.open { transform: rotate(180deg); }
  ::selection { background: #E7F0EA; }
  :focus-visible { outline: 2px solid #3D7A5E; outline-offset: 2px; }
  @media (prefers-reduced-motion: reduce) {
    .accordion-panel, .chev, * { transition: none !important; }
  }
  .scrollbar-thin::-webkit-scrollbar { height: 4px; }
  .scrollbar-thin::-webkit-scrollbar-thumb { background:#D8D4CA; border-radius:4px; }
</style>
</head>
<body class="text-ink antialiased pb-28">

<!-- ================= HEADER / 検索・会社名 ================= -->
<header class="sticky top-0 z-30 bg-paper/95 backdrop-blur border-b border-line">
  <div class="max-w-3xl mx-auto px-4 pt-4 pb-3">
    <div class="flex items-center justify-between gap-3">
      <div class="flex items-baseline gap-2">
        <span class="font-display font-900 text-xl tracking-tight">uFit</span>
        <span class="font-display font-700 text-xs text-inksoft">法人・大口発注フォーム</span>
      </div>
      <span id="lineCount" class="font-num text-xs text-inksoft">119 品中 119 品表示</span>
    </div>

    <div class="mt-3">
      <label for="companyName" class="block text-xs font-700 text-inksoft mb-1">会社名・団体名 <span class="text-danger">必須</span></label>
      <input id="companyName" type="text" placeholder="例）株式会社サンプル / ◯◯ジム"
        class="w-full rounded-lg border border-line bg-white px-3 py-2.5 text-sm focus:border-matcha focus:ring-1 focus:ring-matcha outline-none">
    </div>

    <div class="mt-2.5 relative">
      <svg class="absolute left-3 top-1/2 -translate-y-1/2 w-4 h-4 text-inksoft" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
        <path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-4.35-4.35M17 10a7 7 0 11-14 0 7 7 0 0114 0z"/>
      </svg>
      <input id="searchInput" type="text" inputmode="search" placeholder="商品名・カラー・味で検索（例：抹茶 / グレー / Mat）"
        class="w-full rounded-lg border border-line bg-white pl-9 pr-9 py-2.5 text-sm focus:border-matcha focus:ring-1 focus:ring-matcha outline-none">
      <button id="clearSearch" type="button" aria-label="検索をクリア" class="hidden absolute right-2.5 top-1/2 -translate-y-1/2 text-inksoft hover:text-ink">
        <svg class="w-4 h-4" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
          <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12"/>
        </svg>
      </button>
    </div>
  </div>
</header>

<!-- ================= MAIN ================= -->
<main class="max-w-3xl mx-auto px-4 py-4">
  <p id="noResult" class="hidden text-center text-sm text-inksoft py-12">該当する商品が見つかりませんでした。</p>
  <div id="accordionRoot" class="space-y-3"></div>
</main>

<!-- ================= 合計サマリー（固定バー） ================= -->
<div class="fixed bottom-0 left-0 right-0 z-40 bg-ink text-white shadow-[0_-6px_20px_rgba(0,0,0,0.15)]">
  <div class="max-w-3xl mx-auto px-4 py-3 flex items-center gap-3">
    <div class="flex-1 min-w-0">
      <div class="flex items-baseline gap-2 font-num">
        <span class="text-[11px] text-white/60 font-body">選択中</span>
        <span id="summaryItemCount" class="text-base font-700">0</span>
        <span class="text-[11px] text-white/60 font-body">品</span>
        <span class="text-white/30 mx-0.5">/</span>
        <span class="text-[11px] text-white/60 font-body">合計</span>
        <span id="summaryQtyCount" class="text-base font-700">0</span>
        <span class="text-[11px] text-white/60 font-body">点</span>
      </div>
      <div class="font-num text-lg font-700 leading-tight">¥<span id="summaryTotal">0</span></div>
    </div>
    <button id="submitBtn" type="button"
      class="shrink-0 bg-matcha hover:bg-matchadark active:scale-[0.98] transition rounded-lg px-5 py-3 text-sm font-700 font-display disabled:opacity-40 disabled:cursor-not-allowed">
      この内容で送信
    </button>
  </div>
</div>

<!-- ================= サンクス画面 ================= -->
<div id="thanksScreen" class="hidden fixed inset-0 z-50 bg-paper flex items-center justify-center px-6">
  <div class="max-w-sm w-full text-center">
    <div class="mx-auto mb-5 w-14 h-14 rounded-full bg-matchasoft flex items-center justify-center">
      <svg class="w-7 h-7 text-matcha" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
        <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7"/>
      </svg>
    </div>
    <h2 class="font-display font-900 text-xl mb-2">ご注文ありがとうございました</h2>
    <p class="text-sm text-inksoft leading-relaxed">スプレッドシートおよびGAS側で処理を開始します。<br>担当者よりご連絡するまで、今しばらくお待ちください。</p>
    <button id="backBtn" type="button" class="mt-6 text-sm font-700 text-matcha underline underline-offset-2">フォームに戻る</button>
  </div>
</div>

<!-- ================= 送信中オーバーレイ ================= -->
<div id="loadingOverlay" class="hidden fixed inset-0 z-50 bg-ink/40 flex items-center justify-center">
  <div class="bg-white rounded-xl px-6 py-5 flex items-center gap-3 shadow-lg">
    <svg class="animate-spin w-5 h-5 text-matcha" fill="none" viewBox="0 0 24 24">
      <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
      <path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4z"></path>
    </svg>
    <span class="text-sm font-700">送信しています…</span>
  </div>
</div>

<script>
/* =========================================================
   設定値（Googleフォーム送信先・Entry ID）
   ========================================================= */
const GOOGLE_FORM_URL = "https://docs.google.com/forms/d/e/1FAIpQLSfn_ijCZcJUpXjIFFJHNh45-th-VW3Plt7b7ojgLY3JRA7AiA/formResponse";
const ENTRY_COMPANY   = "entry.1497839987";
const ENTRY_ORDER     = "entry.791195811";

/* =========================================================
   商品マスタデータ（119商品）
   ========================================================= */
const PRODUCTS = [
  { category: "RELEASERシリーズ", name: "uFit RELEASER Mini (White)", price: "¥16,800(税込)" },
  { category: "RELEASERシリーズ", name: "uFit RELEASER Mini (Black)", price: "¥16,800(税込)" },
  { category: "RELEASERシリーズ", name: "【管理医療機器】uFit RELEASER", price: "¥22,800(税込)" },
  { category: "RELEASERシリーズ", name: "uFit RELEASER Pro", price: "¥39,800(税込)" },
  { category: "RELEASERシリーズ", name: "汎用ACアダプタ DC18.0V 1A 18W", price: "¥1,980(税込)" },
  { category: "VIBRATINGシリーズ", name: "uFit Vibrating Roller", price: "¥16,800(税込)" },
  { category: "VIBRATINGシリーズ", name: "uFit Vibrating Roller Mini", price: "¥12,800(税込)" },
  { category: "VIBRATINGシリーズ", name: "uFit Vibrating Ball", price: "¥14,800(税込)" },
  { category: "VIBRATINGシリーズ", name: "uFit Vibrating Ball Mini", price: "¥12,800(税込)" },
  { category: "MATシリーズ", name: "uFit Training Mat 10mm ブラック", price: "¥6,480(税込)" },
  { category: "MATシリーズ", name: "uFit Training Mat 10mm グレー", price: "¥6,480(税込)" },
  { category: "MATシリーズ", name: "uFit Training Mat 10mm ダスティブルー", price: "¥6,480(税込)" },
  { category: "MATシリーズ", name: "uFit Training Mat 15mm ブラック", price: "¥7,980(税込)" },
  { category: "MATシリーズ", name: "uFit Training Mat 15mm グレー", price: "¥7,980(税込)" },
  { category: "MATシリーズ", name: "uFit Training Mat 15mm ダスティブルー", price: "¥7,980(税込)" },
  { category: "MATシリーズ", name: "uFit Training Mat 15mm オガトレコラボ", price: "¥7,980(税込)" },
  { category: "MATシリーズ", name: "uFit Training Mat 15mm ちゃんちーコラボ", price: "¥7,980(税込)" },
  { category: "MATシリーズ", name: "uFit Yoga Mat 4mm ブラック", price: "¥2,980(税込)" },
  { category: "MATシリーズ", name: "uFit Yoga Mat 4mm ダスティブルー", price: "¥2,980(税込)" },
  { category: "MATシリーズ", name: "uFit Yoga Mat 4mm ダスティピンク", price: "¥2,980(税込)" },
  { category: "MATシリーズ", name: "uFit Yoga Mat 4mm オレンジ", price: "¥2,980(税込)" },
  { category: "MATシリーズ", name: "uFit Yoga Mat 4mm ブルー", price: "¥2,980(税込)" },
  { category: "MATシリーズ", name: "uFit Yoga Mat 4mm パープル", price: "¥2,980(税込)" },
  { category: "MATシリーズ", name: "uFit Yoga Mat 4mm ベビーピンク", price: "¥2,980(税込)" },
  { category: "MATシリーズ", name: "uFit Yoga Mat 4mm グレージュ", price: "¥2,980(税込)" },
  { category: "MATシリーズ", name: "uFit Yoga Mat 6mm ブラック", price: "¥3,980(税込)" },
  { category: "MATシリーズ", name: "uFit Yoga Mat 6mm ダスティブルー", price: "¥3,980(税込)" },
  { category: "MATシリーズ", name: "uFit Yoga Mat 6mm ダスティピンク", price: "¥3,980(税込)" },
  { category: "MATシリーズ", name: "uFit ストレッチマット6mm produced by オガトレ", price: "¥3,980(税込)" },
  { category: "MATシリーズ", name: "uFit Exercise Mat 200×90cm グレー", price: "¥4,980(税込)" },
  { category: "MATシリーズ", name: "uFit Exercise Mat 200×90cm ダスティブルー", price: "¥4,980(税込)" },
  { category: "MATシリーズ", name: "uFit Exercise Mat 200×90cm ダスティピンク", price: "¥4,980(税込)" },
  { category: "MATシリーズ", name: "uFit Exercise Mat 200×90cm グレージュ", price: "¥4,980(税込)" },
  { category: "MATシリーズ", name: "uFit Exercise Mat 200×90cm ピンクグレー", price: "¥4,980(税込)" },
  { category: "MATシリーズ", name: "uFit Exercise Mat 183×61cm グレー", price: "¥3,980(税込)" },
  { category: "MATシリーズ", name: "uFit Exercise Mat 183×61cm ダスティブルー", price: "¥3,980(税込)" },
  { category: "MATシリーズ", name: "uFit Exercise Mat 183×61cm ダスティピンク", price: "¥3,980(税込)" },
  { category: "MATシリーズ", name: "uFit Exercise Mat 183×61cm グレージュ", price: "¥3,980(税込)" },
  { category: "MATシリーズ", name: "uFit Exercise Mat 183×61cm ピンクグレー", price: "¥3,980(税込)" },
  { category: "MATシリーズ", name: "Wide Mat ブラック", price: "¥4,980(税込)" },
  { category: "MATシリーズ", name: "Wide Mat ダスティブルー", price: "¥4,980(税込)" },
  { category: "MATシリーズ", name: "Wide Mat グレージュ", price: "¥4,980(税込)" },
  { category: "MATシリーズ", name: "Wide Mat ピンクグレー", price: "¥4,980(税込)" },
  { category: "RECOVERYシリーズ", name: "uFit 磁気ネックレス シルバー45cm", price: "¥9,800(税込)" },
  { category: "RECOVERYシリーズ", name: "uFit 磁気ネックレス シルバー51cm", price: "¥9,800(税込)" },
  { category: "RECOVERYシリーズ", name: "uFit 磁気ネックレス ブラック45cm", price: "¥9,800(税込)" },
  { category: "RECOVERYシリーズ", name: "uFit 磁気ネックレス ブラック51cm", price: "¥9,800(税込)" },
  { category: "RECOVERYシリーズ", name: "uFit 低周波治療器 取り替え専用パッド", price: "¥2,420" },
  { category: "RECOVERYシリーズ", name: "uFit Pocket-Pulse 低周波治療器&マイクロカレント", price: "¥29,800(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Performance pole クールブラック", price: "¥6,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Performance pole ソフトアイボリー", price: "¥6,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Performance pole ダークブルー", price: "¥6,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Performance pole オガトレコラボ", price: "¥6,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Performance pole グレージュ", price: "¥6,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Performance pole ピンクグレー", price: "¥6,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Recovery Ball", price: "¥1,680(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Balance Ball 55cm グレー", price: "¥5,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Balance Ball 55cm ブルー", price: "¥5,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Balance Ball 55cm ブラウン", price: "¥5,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Balance Ball 65cm グレー", price: "¥6,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Balance Ball 65cm ブルー", price: "¥6,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Balance Ball 65cm ブラウン", price: "¥6,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Training Tube Beginner", price: "¥3,480(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Training Tube Expert", price: "¥4,480(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Training Tube Ultimate", price: "¥4,480(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Rubber Tube", price: "¥980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Trampoline グレージュ", price: "¥16,800(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Trampoline コバルトブルー", price: "¥16,800(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Trampoline ブラウン", price: "¥16,800(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Home Bike", price: "¥44,800(税込)" },
  { category: "HOME FITNESSシリーズ", name: "【売り切れ】Foam Roller", price: "¥2,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Bumply Ball 68mm", price: "¥3,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Performance pole Half ソフトアイボリー", price: "¥4,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Performance pole Half クールブラック", price: "¥4,980(税込)" },
  { category: "HOME FITNESSシリーズ", name: "uFit Bumply Ball Mini", price: "¥1,980(税込)" },
  { category: "uFit Soy Protein", name: "750g プレーン", price: "¥4,480" },
  { category: "uFit Soy Protein", name: "750g ココア", price: "¥4,480" },
  { category: "uFit Soy Protein", name: "750g 黒糖きな粉", price: "¥4,480" },
  { category: "uFit Soy Protein", name: "750g カフェオレ", price: "¥4,480" },
  { category: "uFit Soy Protein", name: "750g 抹茶", price: "¥4,480" },
  { category: "uFit Soy Protein", name: "750g ほうじ茶", price: "¥4,480" },
  { category: "uFit Soy Protein", name: "【売り切れ】750g チャイ", price: "¥4,480" },
  { category: "uFit Soy Protein", name: "750g コーピー", price: "¥4,480" },
  { category: "uFit Soy Protein", name: "1.5kg プレーン", price: "¥8,280" },
  { category: "uFit Soy Protein", name: "1.5kg ココア", price: "¥8,280" },
  { category: "uFit Soy Protein", name: "1.5kg 黒糖きな粉", price: "¥8,280" },
  { category: "uFit Soy Protein", name: "1.5kg カフェオレ", price: "¥8,280" },
  { category: "uFit Soy Protein", name: "1.5kg 抹茶", price: "¥8,280" },
  { category: "uFit Soy Protein", name: "1.5kg ほうじ茶", price: "¥8,280" },
  { category: "uFit Soy Protein", name: "【売り切れ】1.5kg チャイ", price: "¥8,280" },
  { category: "uFit完全栄養食", name: "500g 抹茶", price: "¥4,280" },
  { category: "uFit完全栄養食", name: "500g ココア", price: "¥4,280" },
  { category: "uFit完全栄養食", name: "500g 黒糖きな粉", price: "¥4,280" },
  { category: "uFit完全栄養食", name: "500g ほうじ茶", price: "¥4,280" },
  { category: "uFit完全栄養食", name: "1.5kg 抹茶", price: "¥10,800" },
  { category: "uFit完全栄養食", name: "1.5kg ココア", price: "¥10,800" },
  { category: "uFit完全栄養食", name: "1.5kg 黒糖きな粉", price: "¥10,800" },
  { category: "uFit完全栄養食", name: "1.5kg ほうじ茶", price: "¥10,800" },
  { category: "uFit Whey Protein", name: "1kg [抹茶]", price: "¥6,480" },
  { category: "uFit Whey Protein", name: "1kg [チョコレート]", price: "¥6,480" },
  { category: "uFit Whey Protein", name: "1kg [ヨーグルト]", price: "¥6,480" },
  { category: "uFit Whey Protein", name: "1kg [グリーンアップル]", price: "¥6,480" },
  { category: "uFit Whey Protein", name: "1kg [黒糖きな粉]", price: "¥6,480" },
  { category: "uFit Whey Protein", name: "1kg [アロエヨーグルト]", price: "¥6,480" },
  { category: "完全栄養WHEY PROTEIN", name: "1kg [ココア]", price: "¥6,480" },
  { category: "完全栄養WHEY PROTEIN", name: "1kg [バナナ]", price: "¥6,480" },
  { category: "完全栄養WHEY PROTEIN", name: "1kg [ミックスベリー]", price: "¥6,480" },
  { category: "完全栄養WHEY PROTEIN", name: "1kg [ヨーグルト]", price: "¥6,480" },
  { category: "完全栄養WHEY PROTEIN", name: "1kg [黒糖きな粉]", price: "¥6,480" },
  { category: "uFitジュニアプロテイン", name: "uFitジュニアプロテイン [いちご]", price: "¥4,480(税込)" },
  { category: "uFitジュニアプロテイン", name: "uFitジュニアプロテイン [ココア]", price: "¥4,480(税込)" },
  { category: "uFitジュニアプロテイン", name: "uFitジュニアプロテイン [バナナ]", price: "¥4,480(税込)" },
  { category: "uFitジュニアプロテイン", name: "uFitジュニアプロテイン [マスカット]", price: "¥4,480(税込)" },
  { category: "その他", name: "uFit Soy Protein お試し6フレーバーセット", price: "¥1,500(税込)" },
  { category: "その他", name: "完全栄養食お試し4フレーバーセット", price: "¥1,800(税込)" },
  { category: "その他", name: "uFit Whey Protein お試し5フレーバーセット", price: "¥1,250(税込)" },
  { category: "その他", name: "uFit Shaker", price: "¥500(税込)" },
  { category: "その他", name: "uFit Premium EAA 600g すっきりレモン風味", price: "¥4,980" },
  { category: "その他", name: "uFit Premium EAA 600g さっぱりキウイ風味", price: "¥4,980" }
].map((p, i) => ({ ...p, id: i, sold: p.name.includes("売り切れ") }));

/* =========================================================
   状態管理
   ========================================================= */
const quantities = {};                 // { productId: number }
const openCategories = new Set([PRODUCTS[0].category]); // 初期は最初のカテゴリのみ開く

const els = {
  root: document.getElementById('accordionRoot'),
  noResult: document.getElementById('noResult'),
  search: document.getElementById('searchInput'),
  clearSearch: document.getElementById('clearSearch'),
  company: document.getElementById('companyName'),
  lineCount: document.getElementById('lineCount'),
  summaryItemCount: document.getElementById('summaryItemCount'),
  summaryQtyCount: document.getElementById('summaryQtyCount'),
  summaryTotal: document.getElementById('summaryTotal'),
  submitBtn: document.getElementById('submitBtn'),
  thanks: document.getElementById('thanksScreen'),
  backBtn: document.getElementById('backBtn'),
  loading: document.getElementById('loadingOverlay'),
};

// カテゴリの出現順を保持したユニーク配列
const CATEGORIES = [...new Set(PRODUCTS.map(p => p.category))];

function parsePrice(str) {
  const m = String(str).match(/[\d,]+/);
  if (!m) return 0;
  return parseInt(m[0].replace(/,/g, ''), 10) || 0;
}

function escapeHtml(str) {
  return String(str)
    .replace(/&/g, '&amp;').replace(/</g, '&lt;').replace(/>/g, '&gt;')
    .replace(/"/g, '&quot;');
}

/* =========================================================
   レンダリング
   ========================================================= */
function render() {
  const keyword = els.search.value.trim().toLowerCase();
  const isSearching = keyword.length > 0;

  const grouped = CATEGORIES.map(cat => {
    const items = PRODUCTS.filter(p => p.category === cat).filter(p => {
      if (!isSearching) return true;
      return p.name.toLowerCase().includes(keyword) || p.category.toLowerCase().includes(keyword);
    });
    return { cat, items };
  }).filter(g => g.items.length > 0);

  els.lineCount.textContent = isSearching
    ? `119 品中 ${grouped.reduce((s, g) => s + g.items.length, 0)} 品表示`
    : `119 品中 119 品表示`;

  els.noResult.classList.toggle('hidden', grouped.length > 0 || !isSearching);
  els.root.classList.toggle('hidden', grouped.length === 0 && isSearching);

  els.root.innerHTML = grouped.map(({ cat, items }) => {
    const isOpen = isSearching ? true : openCategories.has(cat);
    const selectedInCat = items.filter(p => (quantities[p.id] || 0) > 0).length;

    const rows = items.map(p => {
      const qty = quantities[p.id] || '';
      const disabled = p.sold;
      return `
        <div class="flex items-center gap-3 py-3 px-4 border-t border-line first:border-t-0 ${disabled ? 'opacity-50' : ''}">
          <div class="flex-1 min-w-0">
            <p class="text-sm font-500 leading-snug">${escapeHtml(p.name)}</p>
            <div class="flex items-center gap-2 mt-0.5">
              <span class="font-num text-xs text-inksoft">${escapeHtml(p.price)}</span>
              ${disabled ? '<span class="text-[10px] font-700 text-danger bg-red-50 px-1.5 py-0.5 rounded">売り切れ</span>' : ''}
            </div>
          </div>
          <input
            type="number"
            inputmode="numeric"
            min="0"
            step="1"
            placeholder="0"
            value="${qty}"
            data-id="${p.id}"
            ${disabled ? 'disabled' : ''}
            aria-label="${escapeHtml(p.name)} の数量"
            class="qty-input w-20 text-right font-num text-sm rounded-lg border border-line bg-white px-2 py-2 focus:border-matcha focus:ring-1 focus:ring-matcha outline-none disabled:bg-line/30 disabled:cursor-not-allowed"
          >
        </div>`;
    }).join('');

    return `
      <section class="rounded-xl border border-line bg-white overflow-hidden">
        <button type="button" data-cat="${escapeHtml(cat)}"
          class="cat-toggle w-full flex items-center justify-between gap-3 px-4 py-3.5 text-left"
          aria-expanded="${isOpen}">
          <span class="flex items-center gap-2 min-w-0">
            <span class="font-display font-700 text-sm truncate">${escapeHtml(cat)}</span>
            <span class="font-num text-[11px] text-inksoft shrink-0">${items.length}品${selectedInCat ? ` ・ ${selectedInCat}品選択中` : ''}</span>
          </span>
          <svg class="chev w-4 h-4 text-inksoft shrink-0 ${isOpen ? 'open' : ''}" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"/>
          </svg>
        </button>
        <div class="accordion-panel ${isOpen ? 'open' : ''}">
          ${rows}
        </div>
      </section>`;
  }).join('');

  bindRowEvents();
  updateSummary();
}

function bindRowEvents() {
  els.root.querySelectorAll('.cat-toggle').forEach(btn => {
    btn.addEventListener('click', () => {
      const cat = btn.dataset.cat;
      if (openCategories.has(cat)) openCategories.delete(cat);
      else openCategories.add(cat);
      render();
    });
  });

  els.root.querySelectorAll('.qty-input').forEach(input => {
    input.addEventListener('input', () => {
      const id = Number(input.dataset.id);
      let cleaned = input.value.replace(/[^0-9]/g, '');
      cleaned = cleaned.replace(/^0+(?=\d)/, '');
      input.value = cleaned;
      quantities[id] = cleaned === '' ? 0 : parseInt(cleaned, 10);
      updateSummary();
      // 件数表示（カテゴリ見出し内の「N品選択中」）だけ更新したい場合は再描画が必要だが、
      // 入力体験を優先し、見出し件数はカテゴリ開閉時に再同期する。
    });
    input.addEventListener('blur', () => {
      if (input.value === '') quantities[Number(input.dataset.id)] = 0;
    });
  });
}

function updateSummary() {
  const selected = PRODUCTS.filter(p => (quantities[p.id] || 0) > 0);
  const totalQty = selected.reduce((s, p) => s + quantities[p.id], 0);
  const totalAmount = selected.reduce((s, p) => s + quantities[p.id] * parsePrice(p.price), 0);

  els.summaryItemCount.textContent = selected.length;
  els.summaryQtyCount.textContent = totalQty;
  els.summaryTotal.textContent = totalAmount.toLocaleString('ja-JP');
}

/* =========================================================
   検索
   ========================================================= */
els.search.addEventListener('input', () => {
  els.clearSearch.classList.toggle('hidden', els.search.value.length === 0);
  render();
});
els.clearSearch.addEventListener('click', () => {
  els.search.value = '';
  els.clearSearch.classList.add('hidden');
  render();
  els.search.focus();
});

/* =========================================================
   送信処理
   ========================================================= */
els.submitBtn.addEventListener('click', async () => {
  const companyName = els.company.value.trim();
  if (!companyName) {
    alert('会社名・団体名を入力してください。');
    els.company.focus();
    return;
  }

  const orderItems = PRODUCTS
    .filter(p => (quantities[p.id] || 0) >= 1)
    .map(p => ({ name: p.name, qty: quantities[p.id] }));

  if (orderItems.length === 0) {
    alert('数量が1以上の商品が1件もありません。注文したい商品の数量を入力してください。');
    return;
  }

  const orderJson = JSON.stringify(orderItems);

  const params = new URLSearchParams();
  params.append(ENTRY_COMPANY, companyName);
  params.append(ENTRY_ORDER, orderJson);

  els.submitBtn.disabled = true;
  els.loading.classList.remove('hidden');

  try {
    // GoogleフォームへのPOSTはCORSの制約上 mode:'no-cors' が必須。
    // レスポンス内容は読めない（opaque）ため、fetch自体が例外を投げない限り成功とみなす。
    await fetch(GOOGLE_FORM_URL, {
      method: 'POST',
      mode: 'no-cors',
      headers: { 'Content-Type': 'application/x-www-form-urlencoded' },
      body: params.toString()
    });
    showThanks();
  } catch (err) {
    // ネットワーク自体に到達できない場合（オフライン等）のみここに来る
    console.error('送信エラー:', err);
    alert('通信に失敗しました。ネットワーク接続をご確認の上、もう一度お試しください。');
  } finally {
    els.loading.classList.add('hidden');
    els.submitBtn.disabled = false;
  }
});

function showThanks() {
  document.body.classList.add('overflow-hidden');
  els.thanks.classList.remove('hidden');
}

els.backBtn.addEventListener('click', () => {
  els.thanks.classList.add('hidden');
  document.body.classList.remove('overflow-hidden');
});

/* 初期描画 */
render();
</script>
</body>
</html>
