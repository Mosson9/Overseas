# 原型生成 Prompt 库（Canva 可复用）

> 把每个页面的 Canva 生成 prompt 固化下来,**可复现、可迭代、配额恢复后可一键续出**。
> 生成流程:`generate-design(design_type + query)` → 拿 candidate → `create-design-from-candidate(job_id, candidate_id)` → 得到 view/edit 链接。
> ⚠️ 当前 Canva 账户已触发**配额上限**;待恢复后,直接用下方 query 续生成"待出"页面。

---

## 通用风格基线（已融进各 query，可统一调整）

- **端侧(移动)**:`design_type: your_story`(9:16 竖屏);风格"Premium dark purple-to-navy gradient, luxurious gold accents, subtle Arabic/Islamic geometric pattern, glossy rounded UI, realistic app store screenshot quality, high detail"。
- **后台(桌面)**:`design_type: youtube_thumbnail`(16:9 横屏);风格"Modern enterprise dark dashboard, tables/charts/toggles, realistic SaaS, high detail, professional"。
- 想换品牌色:把 "purple-navy + gold" 换成你的主色,或生成时挂 brand kit。

---

## A. 端侧页面（design_type: your_story）

### A1. 登录页 ✅ 已出
- 查看 https://www.canva.com/d/HCOCNN68JX620N-
- query:
```
High-fidelity mobile app UI mockup, vertical phone screen, for a MENA Arabic voice-chat social app like Yalla. LOGIN screen. Premium dark purple-to-navy gradient, gold accents, subtle Islamic geometric pattern, glowing sound-wave and microphone motifs. Top: app logo circle with name 'VoiceUp'; headline 'Welcome to VoiceUp' + Arabic subtitle 'مرحبا بك'; large gold gradient 'Continue with Phone' button with phone icon; an 'or' divider; a row of three round social buttons (Google, Apple, Facebook); a ghost link 'Continue as Guest'; small grey legal text 'By continuing you agree to Terms & Privacy Policy'. Glossy rounded components, soft glows, realistic app screenshot quality, high detail.
```

### A2. 收银台/充值 ✅ 已出
- 查看 https://www.canva.com/d/qUtyLDoJvTk2ytl
- query:
```
High-fidelity mobile app UI mockup, vertical phone screen, RECHARGE/TOP-UP (cashier) screen for a MENA Arabic voice-chat social app. Premium dark purple-navy gradient, gold accents, Islamic pattern. Top: 'Recharge' title and balance row with gold coin '1,200' and diamond '30'. Middle: 2-column grid of recharge tier cards — first highlighted with 'First Charge +200%' flame badge, others '19 SAR','75 SAR','199 SAR','399 SAR' with bonus coins in gold. Payment rows with radio + logos: 'mada','STC Pay','Apple Pay','Carrier Billing'. Large gold 'Confirm Payment' button. Small grey link 'Payment issue? Contact Support'. Glossy cards, shiny coin/gem icons, realistic app screenshot quality, high detail.
```

### A3. 语音房 ✅ 已出
- 查看 https://www.canva.com/d/-GvbysMfkFTVPml
- query:
```
High-fidelity mobile app UI mockup, vertical phone screen, a live VOICE CHAT ROOM for a MENA Arabic social app like Yalla. Festive warm purple-gold gradient, lively. Top bar: back arrow, room name 'Night Majlis', gold crown host badge, online count '328'. A grid of 8 circular MIC SEATS, avatars in glowing golden rings with sound-wave rings; seat 1 has a crown (host), some filled, two empty with '+'. Middle: public chat with colorful bubbles (one Arabic 'مرحبا'), a system welcome, and a bright GIFT animation of a luxury sports car crossing with 'user_z sent Sports Car'. Small wealth-ranking banner. Bottom toolbar: emoji, gift(gold), mic, message, glowing 'PK' button. Realistic, glossy, colorful, app screenshot quality, high detail.
```

### A4. 主播中台/创作者中心 ✅ 已出
- 查看 https://www.canva.com/d/RcAJD11U3aCGiDT
- query:
```
High-fidelity mobile app UI mockup, vertical phone screen, a STREAMER/HOST earnings console 'Creator Center' for a MENA Arabic voice-chat app. Premium dark purple-navy gradient, gold accents. Top: 'My Earnings' + 'This period'. Large earnings card: gem icon 'Diamonds 52,000 ≈ $248', line 'My split: 55% (floor-protected ✓)' with shield icon, 'Estimated payout: $136'. Itemized breakdown rows: 'Gifts','PK rewards','Hours task'. Gold 'Withdraw' button + note 'This month withdrawn $150' + grey link 'Transparent settlement — view records / Appeal'. Tasks card: 'Live hours 48/60h' gold progress bar, 'PK won 3 matches +reward', daily check-in. Glossy cards, small charts, gem/coin icons, realistic app screenshot quality, high detail.
```

### A5. 钱包页 ⏳ 待出（配额恢复后用此）
- 对应《08 钱包计费中台》6.1
- query:
```
High-fidelity mobile app UI mockup, vertical phone screen, a WALLET screen for a MENA Arabic voice-chat social app. Premium dark purple-to-navy gradient, gold accents. Top: 'My Wallet' title. A glossy balance card with gold coin icon 'Coins 1,200' and diamond icon 'Diamonds 30', and a gold 'Recharge' button. Below a divider 'Streamer Earnings': gem icon 'Diamonds 42,000 ≈ $200' and gold 'Withdraw' button with note 'This month withdrawn $150'. A 'Transaction history' link with three recent rows: recharge (+coins), gift sent (-coins), withdrawal. Glossy rounded cards, shiny coin/gem icons, realistic app store screenshot quality, high detail.
```

---

## B. 后台页面（design_type: youtube_thumbnail）

### B1. 人审工作台 ✅ 已出
- 查看 https://www.canva.com/d/009gegSOVxNjS60
- query:
```
High-fidelity DESKTOP web admin dashboard UI mockup, landscape 16:9, a content-moderation review console for a social live-audio trust & safety team. Dark dashboard, blue/purple accents. Left sidebar (Queue, Reports, Policy, Analytics). Main: a moderation task card 'Ticket #5521 — Voice Room — Level P1', an audio waveform player with timeline/timestamp, a circular risk gauge '0.78 sexual-suggestive', a transcript panel with Arabic + English translation. Action buttons: 'Approve','Warn','Mute','Ban 15d','Permanent Ban', red 'Escalate to P0'. Right KPI panel: 'Accuracy 98.6%','Miss rate 0','SLA on-track'. Top stats bar: 'Pending 38','Handled today 124','Avg time 2.1h'. Realistic enterprise SaaS, tables/charts, high detail.
```

### B2. 运营后台 ✅ 已出
- 查看 https://www.canva.com/d/HPOX29Gwj7q28Cy
- query:
```
High-fidelity DESKTOP web admin dashboard UI mockup, landscape 16:9, an OPERATIONS console for a social live-audio growth/ops team. Dark dashboard, purple/teal accents. Left sidebar (Activities, Resource Slots, Remote Config, A/B Tests, Calendar). Main: 'Activity Management' table rows 'Ramadan Recharge Rebate — Rebate — 2/8-3/10 — Running','New User 7-day Check-in — Running','Weekend PK Battle — Pending'. Side panel 'Resource Slot: Home Banner' with banner thumbnail + audience/time/frequency. A/B card 'First-charge pack v2: A 50% / B 50%, B +18% (96% confidence)' with green 'Roll out B'. Remote-config toggle list with switches. Top bar with app selector + stat cards. Realistic enterprise SaaS, tables/toggles/charts, high detail.
```

### B3. 归因看板 ✅ 已出
- 查看 https://www.canva.com/d/fXuAXLOgkhP5XnB
- query:
```
High-fidelity DESKTOP web analytics dashboard UI mockup, landscape 16:9, a user-acquisition ATTRIBUTION & ROAS dashboard. Dark dashboard, blue/purple/green accents. Top filter bar: App selector, Country, Date range + four KPI tiles: Spend, New Users, CPI, Blended ROAS. Main ROAS table columns 'Channel | Spend | Installs | CPI | D7 ROAS' rows: 'Meta $12,300/8,200/$1.50/0.72','Google UAC/6,100/$1.61/0.65','TikTok/3,500/$1.20/0.81 (green up)','ASA/1,400/$2.21/0.90'. A ROAS trend line chart + a spend-by-channel bar chart. A creative card 'creative SA_H1_v3: CTR 4.1%, reg cost $1.3, D7 ROAS 0.79' with thumbnail. Red alert badge 'Suspected fraud 3.2%'. Realistic enterprise analytics SaaS, high detail.
```

### B4. 公会后台 ✅ 已出
- 查看 https://www.canva.com/d/0tMJXSlVcFfRYt9
- query:
```
High-fidelity DESKTOP web admin dashboard UI mockup, landscape 16:9, a GUILD/AGENCY MANAGEMENT console for a MENA voice-chat ops team. Dark dashboard, purple/gold accents. Left sidebar (Guilds, Anchors, Settlement, Recall, Audit). Main: 'Guild Management' table columns 'Guild | Tier | Anchors | Monthly Flow | Deposit | Status' rows 'GuildAlpha | T1 | 42 | $86,200 | $5,000 | Active','GuildBeta | T2 | 18 | $21,400 | $2,000 | Skimming appeal x2'. Buttons 'Add Guild','Split Config','Penalty'. Side panel: split-ratio config (Platform/Guild/Anchor %) with 'Anchor floor protection' toggle ON. Top stat cards: total guilds, anchors, monthly GMV. Realistic enterprise SaaS, tables/badges, high detail.
```

### B5. 召回 CRM ✅ 已出
- 查看 https://www.canva.com/d/8HkWA7BWfn6p_sg
- query:
```
High-fidelity DESKTOP web admin UI mockup, landscape 16:9, a STREAMER RECALL CRM console for a MENA voice-chat ops team. Dark dashboard, teal/purple accents. Left sidebar. Main: filter bar 'Lifecycle: Churned 7d+' and a recall table columns 'Anchor | Tier | WhatsApp | Silent days | Lifecycle | Status' rows 'A_star | T1 | +966 5XX | 8 days | Growth | To-contact [One-click Recall]','B_voice | T2 | +20 10X | 15 days | Churned | Contacted no reply'. Side panel: recall strategy by stage 'Churned = emotional + comeback gift pack; Silent = exclusive incentive'. A small funnel chart 'Recalled to Returned'. WhatsApp/Push outreach buttons. Realistic enterprise CRM SaaS, status chips, high detail.
```

### B6. 支付/对账后台 ⏳ 待出（配额恢复后用此）
- 对应《03 支付中台》6.2
- query:
```
High-fidelity DESKTOP web admin dashboard UI mockup, landscape 16:9, a PAYMENT & RECONCILIATION console for a social app finance/risk team. Dark dashboard, blue/green accents. Left sidebar (Orders, Reconciliation, Chargebacks, Channels). Main: 'Order Management' table columns 'order_id | user | amount | channel | status | time' with a 'mada / 19 SAR / success' row and a red 'Stripe / 99 USD / Chargeback / [Dispute]' row. A reconciliation panel 'mada today 1,204 txns matched, diff 0'. A chargeback-rate gauge '0.4% (threshold 0.9%) Normal' in green. A channel routing/success-rate panel. Top KPI cards: today revenue, success rate, refunds. Realistic enterprise fintech SaaS, tables/gauges/charts, high detail.
```

### B7. 内容安全策略后台 ⏳ 待出（配额恢复后用此）
- 对应《06 内容安全审核中台》6.2
- query:
```
High-fidelity DESKTOP web admin dashboard UI mockup, landscape 16:9, a CONTENT-SAFETY POLICY console for a social live-audio trust & safety team. Dark dashboard, red/purple accents. Left sidebar (Queue, Reports, Policy, Analytics). Main: a 'Policy Library' for Country = Saudi Arabia, a rules table columns 'Rule | Threshold/Action' rows 'Nudity → 0.5 → P0 instant-cut + permanent ban','Suggestive attire → 0.7 → P1 human review','Political/religious sensitive → match → P0 + report','Minor features → 0.6 → P0 + verify'. A badge 'Gulf strictness = MAX'. A 'Copy to other countries' button. A reports panel 'Today 124, handled 98%, avg time 2.1h'. Top stats: interception volume, miss rate 0. Realistic enterprise trust-and-safety SaaS, tables/threshold sliders, high detail.
```

---

## 续出操作（配额恢复后）
1. 用 ⏳ 待出页面的 query 调 `generate-design`(注意 design_type)。
2. 选一个 candidate,调 `create-design-from-candidate(job_id, candidate_id)` 得 view/edit 链接。
3. 把链接补进 `原型图/README.md` 对应小节。
4. 如需 PNG 落库:在环境网络出口放行 `export-download.canva.com`、`design.canva.ai`,再 `export-design` 下载。
