<!doctype html>
<html lang="zh-CN">
<head>
<meta charset="utf-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover,user-scalable=no"/>
<title>你是 AI 时代的什么人 · 16 型人格测试</title>
<meta name="description" content="12 道题，测你在 AI 创业里是哪种物种。套壳诗人？提示词修仙者？大模型孤勇者？AI 圈人人对号入座。"/>
<meta property="og:title" content="你是 AI 时代的什么人？"/>
<meta property="og:description" content="12 道题 · 16 种 AI 人格 · 测测你在 AI 创业里是哪种物种"/>
<meta property="og:type" content="website"/>
<meta name="twitter:card" content="summary_large_image"/>
<meta name="theme-color" content="#0a0a12"/>
<style>
*{box-sizing:border-box;-webkit-tap-highlight-color:transparent}
html,body{margin:0;padding:0;background:#0a0a12;color:#ecedf5;font-family:-apple-system,"PingFang SC","Microsoft YaHei","Helvetica Neue",sans-serif;-webkit-font-smoothing:antialiased;overflow-x:hidden}
body{min-height:100vh;min-height:100dvh;overscroll-behavior:none}
:root{--accent:#8b5cf6;--accent2:#ec4899;--bg:#0a0a12;--card:rgba(255,255,255,.04);--muted:#7a7e95}
.mono{font-family:"SF Mono","JetBrains Mono",Menlo,Consolas,monospace}
.serif{font-family:"Georgia","Songti SC","SimSun",serif}
/* particle bg */
#bg{position:fixed;inset:0;z-index:0;pointer-events:none;opacity:.5}
/* screens */
.screen{position:relative;z-index:1;min-height:100vh;min-height:100dvh;padding:max(env(safe-area-inset-top),20px) 22px max(env(safe-area-inset-bottom),24px);display:flex;flex-direction:column;animation:fade .5s ease}
@keyframes fade{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:none}}
.hidden{display:none!important}
/* intro */
.intro{justify-content:space-between}
.intro .top{padding-top:6vh}
.brand{font-size:12px;letter-spacing:.3em;color:var(--muted)}
.brand .dot{display:inline-block;width:6px;height:6px;border-radius:50%;background:var(--accent2);margin-right:10px;animation:pulse 1.8s infinite;vertical-align:middle}
@keyframes pulse{0%,100%{opacity:.4}50%{opacity:1}}
.title{font-size:44px;line-height:1.05;font-weight:800;margin:22px 0 14px;letter-spacing:-.02em}
.title .grad{background:linear-gradient(135deg,#f0abfc,#8b5cf6 50%,#22d3ee);-webkit-background-clip:text;background-clip:text;color:transparent}
.sub{color:#b7bace;font-size:15px;line-height:1.7;max-width:480px}
.meta{display:flex;gap:16px;margin-top:26px;font-size:12px;color:var(--muted);letter-spacing:.15em}
.meta span b{color:#e0e2ee;font-weight:600}
.hook{margin-top:28px;padding:14px 16px;border:1px solid rgba(255,255,255,.08);border-radius:14px;background:var(--card);font-size:13.5px;line-height:1.7;color:#c9ccdd}
.hook b{color:#f0abfc}
.btn{display:flex;align-items:center;justify-content:center;gap:10px;padding:17px 20px;border-radius:14px;font-size:16px;font-weight:600;letter-spacing:.05em;border:none;cursor:pointer;width:100%;transition:transform .15s,box-shadow .2s}
.btn:active{transform:scale(.98)}
.btn-primary{background:linear-gradient(135deg,var(--accent),var(--accent2));color:#fff;box-shadow:0 10px 30px rgba(139,92,246,.35)}
.btn-ghost{background:rgba(255,255,255,.06);color:#ecedf5;border:1px solid rgba(255,255,255,.1)}
.btn-row{display:flex;gap:10px}
.btn-row .btn{flex:1}
.intro .cta{margin-top:auto;padding-top:24px}
.footer-hint{text-align:center;font-size:11px;color:var(--muted);margin-top:12px;letter-spacing:.15em}
/* question */
.qwrap{flex:1;display:flex;flex-direction:column;padding-top:8px}
.progress{display:flex;gap:4px;margin-bottom:22px}
.progress span{flex:1;height:3px;background:rgba(255,255,255,.08);border-radius:2px;overflow:hidden;position:relative}
.progress span.done::after,.progress span.cur::after{content:"";position:absolute;inset:0;background:linear-gradient(90deg,var(--accent),var(--accent2));border-radius:2px}
.qnum{font-size:12px;color:var(--muted);letter-spacing:.3em}
.qemoji{font-size:42px;margin:18px 0 12px;animation:bounce .6s}
@keyframes bounce{0%{transform:scale(.5)}60%{transform:scale(1.15)}100%{transform:scale(1)}}
.qtext{font-size:22px;line-height:1.45;font-weight:700;margin-bottom:4px;max-width:540px}
.qhint{color:var(--muted);font-size:13px;letter-spacing:.05em;margin-bottom:26px}
.opts{display:flex;flex-direction:column;gap:12px;margin-top:auto;padding-bottom:12px}
.opt{padding:18px 18px;border-radius:16px;background:var(--card);border:1.5px solid rgba(255,255,255,.08);cursor:pointer;transition:all .2s;display:flex;gap:14px;align-items:flex-start;font-size:15.5px;line-height:1.5;text-align:left;color:#dde0ef;font-family:inherit;width:100%}
.opt:active{transform:scale(.98);border-color:var(--accent)}
.opt .mark{width:28px;height:28px;border-radius:50%;background:rgba(255,255,255,.06);display:flex;align-items:center;justify-content:center;font-size:12px;font-weight:700;color:#fff;flex-shrink:0;margin-top:1px;font-family:var(--mono)}
.opt.pick{border-color:var(--accent);background:rgba(139,92,246,.12)}
.opt.pick .mark{background:linear-gradient(135deg,var(--accent),var(--accent2))}
/* loading */
.load{justify-content:center;align-items:center;text-align:center}
.load .ring{width:100px;height:100px;border-radius:50%;border:3px solid rgba(255,255,255,.08);border-top-color:var(--accent2);animation:spin 1s linear infinite;margin-bottom:30px}
@keyframes spin{to{transform:rotate(360deg)}}
.load .t{font-size:17px;font-weight:700;letter-spacing:.05em;margin-bottom:18px}
.load .log{font-family:var(--mono);font-size:12.5px;color:var(--muted);line-height:1.9;text-align:left;max-width:320px;width:100%;background:rgba(0,0,0,.3);padding:14px 16px;border-radius:10px;border:1px solid rgba(255,255,255,.05);min-height:140px}
.load .log b{color:#7cf6c8;font-weight:400}
.load .log .ok{color:#7cf6c8}
/* result */
.result{padding-bottom:60px}
.rhead{text-align:center;padding:20px 0 10px}
.rcode{font-family:var(--mono);font-size:clamp(76px,22vw,120px);font-weight:900;line-height:1;letter-spacing:-.03em;margin:8px 0;background:linear-gradient(135deg,var(--c1,#f0abfc),var(--c2,#22d3ee));-webkit-background-clip:text;background-clip:text;color:transparent;position:relative}
.rcode::after{content:attr(data-code);position:absolute;inset:0;background:linear-gradient(135deg,var(--c1,#f0abfc),var(--c2,#22d3ee));-webkit-background-clip:text;background-clip:text;color:transparent;filter:blur(18px);opacity:.5;z-index:-1}
.rname{font-size:28px;font-weight:800;margin:6px 0 4px;letter-spacing:-.01em}
.ren{font-size:12px;color:var(--muted);letter-spacing:.3em;text-transform:uppercase}
.rtag{display:inline-block;margin-top:14px;padding:5px 14px;border-radius:99px;font-size:11.5px;letter-spacing:.25em;background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.1);color:#c9ccdd;font-family:var(--mono)}
.sec{margin-top:22px;padding:22px 20px;border-radius:18px;background:var(--card);border:1px solid rgba(255,255,255,.06);position:relative;overflow:hidden;animation:rise .6s backwards}
.sec:nth-child(2){animation-delay:.1s}.sec:nth-child(3){animation-delay:.2s}.sec:nth-child(4){animation-delay:.3s}.sec:nth-child(5){animation-delay:.4s}.sec:nth-child(6){animation-delay:.5s}
@keyframes rise{from{opacity:0;transform:translateY(20px)}to{opacity:1;transform:none}}
.sec h3{font-size:11px;letter-spacing:.3em;color:var(--muted);margin:0 0 12px;font-weight:600;text-transform:uppercase}
.sec h3 .e{margin-right:8px;font-size:14px}
.sec p{margin:0;font-size:15px;line-height:1.75;color:#dde0ef}
.sec .serif{font-family:"Georgia","Songti SC",serif}
.pair{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-top:4px}
.pair .box{padding:12px 12px;border-radius:12px;background:rgba(0,0,0,.2);border:1px solid rgba(255,255,255,.05)}
.pair .box .lbl{font-size:10.5px;letter-spacing:.2em;color:var(--muted);margin-bottom:6px;font-family:var(--mono)}
.pair .box .val{font-size:14px;font-weight:600;color:#ecedf5;line-height:1.4}
.pair .box .code{font-family:var(--mono);font-size:11px;color:var(--c1);margin-top:3px}
.pair .good{border-color:rgba(124,246,200,.2)} .pair .good .lbl{color:#7cf6c8}
.pair .bad{border-color:rgba(255,122,184,.2)} .pair .bad .lbl{color:#ff7ab8}
.death{background:linear-gradient(135deg,rgba(255,122,184,.08),rgba(239,68,68,.08));border-color:rgba(255,122,184,.2)}
.next{background:linear-gradient(135deg,rgba(124,246,200,.08),rgba(34,211,238,.08));border-color:rgba(124,246,200,.2)}
.share-bar{position:sticky;bottom:0;left:0;right:0;margin:28px -22px -24px;padding:16px 22px calc(max(env(safe-area-inset-bottom),14px) + 4px);background:linear-gradient(to top,var(--bg) 60%,transparent);display:flex;flex-direction:column;gap:10px;z-index:10}
.counter{text-align:center;font-size:12px;color:var(--muted);letter-spacing:.1em;margin-top:12px}
.counter b{color:#f0abfc;font-family:var(--mono)}
/* modal */
.modal{position:fixed;inset:0;z-index:100;background:rgba(0,0,0,.8);backdrop-filter:blur(20px);display:flex;align-items:center;justify-content:center;padding:20px;animation:fade .3s}
.modal .card{background:#151524;border:1px solid rgba(255,255,255,.1);border-radius:20px;padding:22px;max-width:420px;width:100%;max-height:92vh;overflow-y:auto}
.modal h4{margin:0 0 14px;font-size:17px}
.modal canvas{width:100%;border-radius:14px;display:block;margin-bottom:14px;box-shadow:0 12px 40px rgba(0,0,0,.5)}
.modal .tip{font-size:12.5px;color:var(--muted);text-align:center;line-height:1.6;margin:8px 0 14px}
.copyln{display:flex;gap:8px;padding:10px 12px;background:rgba(0,0,0,.3);border-radius:10px;border:1px solid rgba(255,255,255,.06);margin-bottom:10px;font-family:var(--mono);font-size:12px;color:#b7bace;align-items:center}
.copyln span{flex:1;overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
.copyln button{all:unset;cursor:pointer;color:#f0abfc;font-size:11px;letter-spacing:.1em;font-weight:600}
.brag{padding:14px;background:rgba(0,0,0,.3);border-radius:12px;border:1px dashed rgba(255,255,255,.15);font-size:13.5px;line-height:1.75;color:#dde0ef;white-space:pre-line;margin-bottom:12px;font-family:var(--mono)}
/* compare */
.compare-input{width:100%;padding:14px;border-radius:12px;border:1.5px solid rgba(255,255,255,.1);background:rgba(0,0,0,.3);color:#ecedf5;font-family:var(--mono);font-size:15px;letter-spacing:.2em;text-align:center;text-transform:uppercase;margin-bottom:12px;outline:none}
.compare-input:focus{border-color:var(--accent)}
.relation{padding:18px;border-radius:14px;background:linear-gradient(135deg,rgba(139,92,246,.1),rgba(236,72,153,.1));border:1px solid rgba(255,255,255,.1);margin-top:10px}
.relation .v{font-size:22px;font-weight:800;margin-bottom:8px;text-align:center}
.relation .d{font-size:14px;line-height:1.7;color:#dde0ef}
/* toast */
.toast{position:fixed;bottom:40px;left:50%;transform:translateX(-50%);background:#fff;color:#0a0a12;padding:10px 18px;border-radius:24px;font-size:13px;font-weight:600;z-index:200;animation:toast 2s forwards;box-shadow:0 10px 40px rgba(0,0,0,.3)}
@keyframes toast{0%{opacity:0;transform:translate(-50%,20px)}15%,85%{opacity:1;transform:translate(-50%,0)}100%{opacity:0;transform:translate(-50%,-10px)}}
/* egg ribbon */
.egg{position:absolute;top:-1px;right:-1px;background:linear-gradient(135deg,#fbbf24,#f59e0b);color:#0a0a12;font-size:10px;font-weight:800;letter-spacing:.15em;padding:4px 10px;border-radius:0 18px 0 12px;font-family:var(--mono)}
@media(min-width:720px){.screen{max-width:560px;margin:0 auto}.title{font-size:56px}}
</style>
</head>
<body>
<canvas id="bg"></canvas>

<!-- INTRO -->
<section class="screen intro" id="s-intro">
	<div class="top">
		<div class="brand"><span class="dot"></span>AI · PERSONA · TEST · v1.0</div>
		<h1 class="title">你是 AI 时代的<br><span class="grad">什么人？</span></h1>
		<p class="sub">12 道题，4 个维度，16 种 AI 创业者人格。<br>测测你在这个时代是哪种物种——以及，你会死于什么。</p>
		<div class="meta"><span><b>12</b> 题</span><span><b>2</b> 分钟</span><span><b>16+</b> 人格</span></div>
		<div class="hook">🧬 套壳诗人、提示词修仙者、GitHub Trending 钉子户、AI Agent 传教士……<br>看看 <b>AI 圈到底把你塑造成了什么样子</b>。</div>
	</div>
	<div class="cta">
		<button class="btn btn-primary" onclick="start()">开始测试 →</button>
		<div class="footer-hint">提示：AI 圈人一看你的代号就懂你</div>
	</div>
</section>

<!-- QUESTION -->
<section class="screen hidden" id="s-q">
	<div class="qwrap">
		<div class="progress" id="prog"></div>
		<div class="qnum" id="qnum">QUESTION 01 / 12</div>
		<div class="qemoji" id="qemoji">🧑‍💻</div>
		<div class="qtext" id="qtext"></div>
		<div class="qhint">选最像你的那个，别装</div>
		<div class="opts" id="opts"></div>
	</div>
</section>

<!-- LOADING -->
<section class="screen load hidden" id="s-load">
	<div class="ring"></div>
	<div class="t">正在分析你的 AI 基因…</div>
	<div class="log" id="loadlog"></div>
</section>

<!-- RESULT -->
<section class="screen hidden" id="s-result"></section>

<script>
/* ========= DATA ========= */
const DIMS = ["MA","HD","ST","OC"]; // M/A, H/D, S/T, O/C

const Q = [
	{e:"🧑‍💻🌙☕", t:"凌晨三点，你在：", a:{t:"疯狂改 prompt，这次一定通",d:"A"}, b:{t:"盯着 loss 曲线祈祷",d:"M"}, dim:"MA"},
	{e:"🪞💬", t:"有人说你做的是套壳：", a:{t:"对，套得很好，下一个问题",d:"A"}, b:{t:"我在训自己的底座，只是还没发",d:"M"}, dim:"MA"},
	{e:"🎓🤖", t:"朋友问你什么是 Transformer：", a:{t:"一种让 AI 变聪明的魔法",d:"A"}, b:{t:"掏出白板开始画 attention",d:"M"}, dim:"MA"},
	{e:"🚀🔥", t:"老黄发布新 GPU，你的第一反应：", a:{t:"冲去预售页面狂刷 F5",d:"H"}, b:{t:"看看能不能跑我那个冷门模型",d:"D"}, dim:"HD"},
	{e:"💣🏳️", t:"OpenAI 发新功能覆盖了你的产品：", a:{t:"完了，删库跑路",d:"H"}, b:{t:"无所谓，我做的是它永远不碰的脏活",d:"D"}, dim:"HD"},
	{e:"🗺️📌", t:"你的产品路线图是怎么定的？", a:{t:"跟着 X Trending 每周变",d:"H"}, b:{t:"两年前就决定好了，不动摇",d:"D"}, dim:"HD"},
	{e:"👯📣", t:"队友说「要不我们加个 Agent」：", a:{t:"好，我连夜写，多谢 idea",d:"T"}, b:{t:"别碰我代码，我自己搞",d:"S"}, dim:"ST"},
	{e:"💼🤝", t:"VC 问你团队情况：", a:{t:"5 个合伙人，缺一个都不行",d:"T"}, b:{t:"我 + Cursor + 一只猫",d:"S"}, dim:"ST"},
	{e:"📆🎮", t:"你的周末通常在：", a:{t:"和联创开会复盘 + 约饭",d:"T"}, b:{t:"一个人戴耳机写到天亮",d:"S"}, dim:"ST"},
	{e:"💰🛡️", t:"VC 问你护城河：", a:{t:"开源社区 3.2k star，社区即壁垒",d:"O"}, b:{t:"8 个付费客户 + NDA，闭嘴赚钱",d:"C"}, dim:"OC"},
	{e:"🍴📦", t:"有人 fork 了你的项目：", a:{t:"欢迎 PR，一起干",d:"O"}, b:{t:"先发个律师函压压惊",d:"C"}, dim:"OC"},
	{e:"💸🏷️", t:"你的产品定价：", a:{t:"免费 + 打赏 + 求个 star",d:"O"}, b:{t:"$99/月起步，企业版另算",d:"C"}, dim:"OC"}
];

const LOAD_LOGS = [
	"扫描你的 GitHub commit 时间分布…",
	"检测 prompt 历史里的「Act as」数量…",
	"分析你的套壳系数 ρ…",
	"追踪你上个月 pivot 的次数…",
	"爬取你关注的 AI KOL 列表…",
	"统计你的 demo day 出席率…",
	"测算你对 AGI 的信仰强度…",
	"匹配 AI 创业者物种数据库…",
	"✓ 基因序列解析完毕"
];

/* ========= 16 PERSONAS ========= */
const P = {
	MHSC:{n:"大模型孤勇者",en:"The Lone Foundation Builder",tag:"自己训 7B 底座，靠信仰发电。",
		desc:"别人在套壳，你在 pretrain。别人在 demo day 讲故事，你在等 loss 收敛。显卡账单比房租贵，冰箱三个月没换过东西。你相信六个月后，全世界都绕不过你——前提是你能撑过这六个月。",
		real:"你押的是最难也最长的赛道。真正能做出底座的人屈指可数，一旦做成护城河极深。但大多数独狼不是死于技术，是死于算力成本和时间窗关闭。你的真正风险是钱和耐心，不是智商。",
		mate:"MDTC",mateN:"闭门修炼派掌门",foe:"AHSC",foeN:"套壳诗人",
		death:"第 7 次预训练时，OpenAI 发了免费同规模模型。",
		next:"别等完美，先开源一个 tokenizer 或 eval 集抢话语权。",c1:"#f0abfc",c2:"#8b5cf6"},
	MHTC:{n:"国产替代总设计师",en:"The Benchmark Gladiator",tag:"PPT 里永远有一张「全球第一」的图。",
		desc:"你的模型每周都刷新一次 SOTA，虽然是在一个没人用的 benchmark 上。路演时你永远能画出五维雷达图，且你家总是最外那一圈。融资材料封面：「对标 GPT-4，部分指标超越」。",
		real:"你吃到了政策和国产化的红利，但也被它绑架。真正的挑战是：benchmark 之外的真实用户体验、可持续的算力供给、以及别的「国产替代」随时追上来。护城河要在生态而不是榜单。",
		mate:"ADTC",mateN:"交付型 AI 服务商",foe:"MDSO",foeN:"独立研究员",
		death:"benchmark 换了标准，你的第一不见了。",
		next:"挑 1 个真实场景做到不可替代，比刷 10 个榜更值钱。",c1:"#fb7185",c2:"#ef4444"},
	MHSO:{n:"开源圣人 · 凌晨三点版",en:"The Midnight Maintainer",tag:"Star 数即生命值，Issue 回复速度即心跳。",
		desc:"白天正经工作，晚上是 repo 之神。GitHub Trending 是你的夜店，contributor 是你的朋友。你的 README 比你的简历长，你的 Discord 成员比你的微信好友多，但你还是没想好怎么赚钱。",
		real:"你积累的社区资产极为珍贵，这是 AI 时代最稀缺的分发渠道。但开源项目的商业化永远是深渊——别被「做大做强再说」骗了，最好的时机就是 star 破万那一刻。",
		mate:"MDTO",mateN:"学院派开源战神",foe:"ADTC",foeN:"交付型 AI 服务商",
		death:"star 10k 那天，你被裁员，但你还在回 issue。",
		next:"立刻推一个 Pro 版或托管服务，别再犹豫。",c1:"#86efac",c2:"#22c55e"},
	MHTO:{n:"Hugging Face 布道团团长",en:"The License Evangelist",tag:"口头禅：「这个 license 不太行」。",
		desc:"你不写代码，你写 license。你不发模型，你发 model card。你在各大社区疯狂转发新开源模型，比作者本人还激动。你的梦想是有一天 Clem 会 follow 你。",
		real:"你是生态的润滑剂，连接上游模型和下游应用。这个位置信息差套利空间极大，但也最容易被视作「不创造价值」。把你的连接能力变成产品（榜单、评测、分发）才是出路。",
		mate:"AHTO",mateN:"AI Agent 传教士",foe:"MDTC",foeN:"闭门修炼派掌门",
		death:"某天 HF 宕机 6 小时，你发现自己没事可做。",
		next:"把你的推荐品味产品化：做榜单，做 newsletter，做评测。",c1:"#fde047",c2:"#eab308"},
	MDSC:{n:"深井 Infra 苦行僧",en:"The Deep Infra Monk",tag:"3 年没换发型，GPU 换了 4 代。",
		desc:"你研究的东西没人听得懂：vLLM、FlashAttention、PagedKV、Speculative Decoding。别人在做产品，你在榨性能。你的工位像考古现场，但你每次提交都能让推理成本降 20%。",
		real:"你做的是真正的硬壁垒，LLM 时代最值钱的岗位之一。但你最容易的陷阱是：只懂工程不懂客户。走出 terminal，让你的优化对接到一个付费场景——你的性价比会让所有人闭嘴。",
		mate:"MDTC",mateN:"闭门修炼派掌门",foe:"AHSC",foeN:"套壳诗人",
		death:"你把推理成本降到 0，但公司没客户。",
		next:"找 1 个高并发 AI 产品做技术合伙人，别自己创业。",c1:"#60a5fa",c2:"#2563eb"},
	MDTC:{n:"闭门修炼派掌门",en:"The Silent Scholar",tag:"不发 demo，不接受采访，只出论文。",
		desc:"你家公司三年没发新闻稿，官网只有一个 email。你融了一轮大钱然后人间蒸发。圈内只有三四个人知道你在干嘛，他们都不敢说。你在等一个巨大的、足以改变叙事的发布。",
		real:"这是最危险也最高回报的路径：Anthropic、DeepMind 都是这种节奏。但 99% 的「闭门修炼」最后没憋出来——你需要时间、钱、顶级人才同时到位。缺一样都是 100 分变 0 分。",
		mate:"MHSC",mateN:"大模型孤勇者",foe:"AHTC",foeN:"流量 AI 产品经理",
		death:"发布会前一周，竞品先发了同样的东西。",
		next:"设一个 hard deadline，否则你会永远不发。",c1:"#c4b5fd",c2:"#7c3aed"},
	MDSO:{n:"独立研究员",en:"The Independent Vibe Researcher",tag:"Bio：just vibing with transformers。",
		desc:"你没有公司，没有团队，没有 title。你只有一台 4090 和一个 Substack。你每周发一篇论文解读，每月放一个玩具 repo，没人知道你怎么活下来的，但你活得很滋润。",
		real:"你走的是最自由的路径：个人品牌即职业安全。风险是收入不稳定、影响力天花板低、容易在 28 岁焦虑。把你的品味和输出结构化——训练营、付费研究、顾问——现金流会稳很多。",
		mate:"ADSO",mateN:"提示词修仙者",foe:"MHTC",foeN:"国产替代总设计师",
		death:"某天你发现你已经 3 个月没收入了，但 Twitter 粉丝涨了 2000。",
		next:"开一个付费 newsletter 或训练营，把声誉变现金。",c1:"#5eead4",c2:"#14b8a6"},
	MDTO:{n:"学院派开源战神",en:"The Academic Crusader",tag:"一边发 paper 一边骂同行。",
		desc:"你的引用量碾压圈内，你的脾气也是。你相信「model weights wants to be free」。你每次开源新 SOTA 都能让商业公司原地打转。你的推文都带「This is embarrassing.」。",
		real:"你是 AI 公共知识最重要的推动者之一。但学院派进入产业的通病是：对商业残酷性估计不足、容易被 PR 伤自尊。把你的声誉资产绑定到一个机构或产品上，而不是只做自己。",
		mate:"MHSO",mateN:"开源圣人 · 凌晨三点版",foe:"AHTC",foeN:"流量 AI 产品经理",
		death:"你发了最强开源模型，三天后被一家创业公司封装收 $200/月。",
		next:"要么加入一家你真正相信的公司，要么自己起盘。别一直单飞。",c1:"#93c5fd",c2:"#3b82f6"},
	AHSC:{n:"套壳诗人",en:"The Wrapper Poet",tag:"用 20 个 prompt 撑起一个独角兽梦。",
		desc:"你的产品核心是一段 system prompt + 一张精修 landing page。你的差异化是 UI 和文案，你的壁垒是「我们更懂用户」。你上周估值 1000 万美金，这周 OpenAI 发了 GPTs。",
		real:"别被「套壳」两个字 PUA。真正厉害的 AHSC 懂用户、懂分发、懂付费——这些能力 OpenAI 永远做不到。但你必须比模型迭代快一步：要么深挖一个垂直，要么跑赢巨头。站在中间必死。",
		mate:"AHTC",mateN:"流量 AI 产品经理",foe:"MHSC",foeN:"大模型孤勇者",
		death:"OpenAI 上线了一个免费版，一模一样，还更好用。",
		next:"把用户数据和工作流做深，别只做 prompt。",c1:"#f9a8d4",c2:"#ec4899"},
	AHTC:{n:"流量 AI 产品经理",en:"The Trend Chaser PM",tag:"上周做 AI 女友，这周做 AI 塔罗。",
		desc:"你在 TikTok 蹲新梗，你在小红书测新痛点。你的产品一个月迭代 5 个方向。你没有长期规划，你有的是 day-by-day 增长黑客的肌肉记忆。你相信「风口比天赋重要」。",
		real:"你对流量的嗅觉是稀缺资源，AI 时代的分发成本急剧下降，短平快能真的赚到钱。但你最大风险是：永远没有沉淀。选一个方向坚持 12 个月，能让你从「流量玩家」变成「行业玩家」。",
		mate:"AHSO",mateN:"GitHub Trending 钉子户",foe:"MDTC",foeN:"闭门修炼派掌门",
		death:"你跑赢了 10 个风口，没一个留下。",
		next:"把最好的那个做深，剩下都卖掉或关掉。",c1:"#fdba74",c2:"#f97316"},
	AHSO:{n:"GitHub Trending 钉子户",en:"The Serial Trender",tag:"每周新 repo 冲榜，没一个留存。",
		desc:"你的 GitHub 首页像博物馆：AutoXXX、AgentYYY、AwesomeZZZ……每个都 star 上千。你每个周末做一个新项目，每周一又开始新的。你是 README 炼金术士，你的 demo gif 是艺术。",
		real:"你的 build in public 能力极其稀缺，这是新一代的自我营销。但从「项目人」到「公司人」需要一次跃迁：选一个 repo 认真做商业化，才能把流量变成现金。不然你永远是个永动机。",
		mate:"MDSO",mateN:"独立研究员",foe:"ADSC",foeN:"垂直行业潜伏者",
		death:"你第 40 个冲榜的 repo 爆了，但你 3 周后就没人记得。",
		next:"挑 star 最高的那个，关掉其他，认真做 6 个月。",c1:"#fcd34d",c2:"#f59e0b"},
	AHTO:{n:"AI Agent 传教士",en:"The Agentic Preacher",tag:"相信 Agent 会替代一切，包括自己。",
		desc:"你的推文里每 3 条有 1 条是 Agent。你做的产品叫 XX-GPT / XX-Agent / Auto-XX。你 demo 一跑十分钟，观众不敢眨眼。你每次都说「这次真的不一样了」。",
		real:"Agent 是 2025-2027 最大的叙事窗口，早期玩家可以拿到巨大红利。但当前技术极不稳定，demo 和产品之间差 100 倍的工程量。你要么做真的能跑的窄场景 agent，要么做底层协议，别停在 demo。",
		mate:"MHTO",mateN:"Hugging Face 布道团团长",foe:"ADSC",foeN:"垂直行业潜伏者",
		death:"你的 Agent demo 永远是那三个步骤，第四步一定崩。",
		next:"挑一个 5 分钟能稳定跑完的场景做到极致，别再加步骤。",c1:"#a5f3fc",c2:"#06b6d4"},
	ADSC:{n:"垂直行业潜伏者",en:"The Vertical Whisperer",tag:"在你没听过的 SaaS 里做到盈利。",
		desc:"你不发 Twitter，你不参加 Demo Day，你不融资。你在一个你大学学的土到不行的行业里，默默用 AI 省下了一整个部门。你年入 300 万美金，没人知道你是谁。",
		real:"你是 AI 时代最被低估的赢家。垂直行业 + AI 的组合护城河极深，远离泡沫。唯一的风险是：太低调导致无法规模化。适度建立个人品牌，你能从 300 万做到 3000 万。",
		mate:"ADTC",mateN:"交付型 AI 服务商",foe:"AHSO",foeN:"GitHub Trending 钉子户",
		death:"你被一个同样垂直但更会营销的人挤掉。",
		next:"把你的 know-how 写成公开内容，建立行业第一品牌。",c1:"#bef264",c2:"#65a30d"},
	ADTC:{n:"交付型 AI 服务商",en:"The AI Delivery Mercenary",tag:"不讲 AI，只讲「我帮你省了多少人」。",
		desc:"你不是 AI 公司，你是咨询公司。你把 GPT、Claude、Cursor、n8n 组合成一套解决方案卖给客户，按人头计费。你在甲方眼里是魔法师，在同行眼里是「就是个外包吧」。",
		real:"你是 AI 最快赚到钱的姿势之一：现金流健康、需求真实、交付可控。但天花板在于「人效」——如果不产品化，你永远在卖自己的时间。把 SOP 变成工具，把工具变成 SaaS，才能跳出外包身份。",
		mate:"ADSC",mateN:"垂直行业潜伏者",foe:"MHSO",foeN:"开源圣人 · 凌晨三点版",
		death:"客户学会了，自己雇了一个你。",
		next:"把最常交付的那个流程做成 SaaS，开始卖订阅。",c1:"#fca5a5",c2:"#dc2626"},
	ADSO:{n:"提示词修仙者",en:"The Prompt Alchemist",tag:"一个 .md 文件值 10 万块。",
		desc:"你的桌面全是 .md 文件：system_v37_final_FINAL.md。你坚信 prompt engineering 是一门手艺、一种哲学、一种修行。你能用一段 prompt 做出别人一整个团队做的事。你的知识库是你的道场。",
		real:"你掌握的其实是「如何驯化大模型」的暗知识，这是 AI 时代最隐形但最值钱的能力。但 prompt 的半衰期在缩短——把你的 prompt 集做成产品（模板站、训练营、Agent 工作流）才能穿越模型迭代。",
		mate:"MDSO",mateN:"独立研究员",foe:"MHSC",foeN:"大模型孤勇者",
		death:"GPT-6 发布，一句话 prompt 就能做你之前 20 行 prompt 的事。",
		next:"把你的 prompt 集打包卖钱，或封装成 Agent 工作流。",c1:"#ddd6fe",c2:"#8b5cf6"},
	ADTO:{n:"开源工作流教主",en:"The Workflow Messiah",tag:"你用过他的 n8n 模板但你不知道。",
		desc:"你不训模型，你不写 prompt，你连 Python 都懒得用。你用 n8n、Dify、Coze、Make 拼出奇迹。你的教程被几万人照着抄，但你不卖课，你卖模板包，299 一个。",
		real:"低代码 AI 工作流是非技术创业者的最佳入口，市场远未饱和。你的优势是把复杂 AI 能力包装给普通用户。别小看这层，这是未来 5 年最大的「软件的二次分发」赛道。",
		mate:"AHTO",mateN:"AI Agent 传教士",foe:"MDSC",foeN:"深井 Infra 苦行僧",
		death:"n8n 推出官方模板市场，免费。",
		next:"从卖模板升级到做托管服务，别停在下载链接。",c1:"#67e8f9",c2:"#0891b2"}
};

/* ========= EGGS ========= */
const EGGS = {
	VC:{n:"VC 观察员 👁️",en:"The Spectator",tag:"你其实不是创业者，你是来看戏的。",
		desc:"你每场发布会都到，每个群都在，每个项目你都「略有了解」。你不下场，但你比谁都懂。你的微信备注是一部 AI 圈通讯录。",
		real:"信息差和人脉是你最大的资产，但永远站在岸上也意味着永远拿不到 carry 之外的巨大回报。选一个你真正相信的项目深度绑定，比 follow 100 个项目都值钱。",
		mate:"MDTC",mateN:"闭门修炼派掌门",foe:"MHSC",foeN:"大模型孤勇者",
		death:"你错过了所有下场的窗口，只剩朋友圈截图。",
		next:"选 1 个项目 all in，从 observer 变成 operator。",c1:"#fde68a",c2:"#d97706"},
	FOG:{n:"还在找方向 🌫️",en:"The Wanderer",tag:"每天读 100 篇 AI 文章，不知道自己要干什么。",
		desc:"你的收藏夹有 800 个 repo，你的稍后读有 2000 篇文章，你的笔记有 50 个「可能的方向」。你每天醒来都觉得自己要开始了，但每晚都没开始。",
		real:"你不是懒，你是选择过载。AI 时代信息爆炸反而让行动变得更难。停止调研，选一个「不完美但真实」的问题，用 2 周时间做一个 demo——你会发现 80% 的焦虑来自不动手。",
		mate:"ADSO",mateN:"提示词修仙者",foe:"AHSO",foeN:"GitHub Trending 钉子户",
		death:"你在第 99 次 pivot 时发现时间已经过了 2 年。",
		next:"今晚就选一个方向，2 周内跑出一个 demo，不许再调研。",c1:"#e5e7eb",c2:"#9ca3af"}
};

/* ========= STATE ========= */
let ans = [], qi = 0;

/* ========= BG PARTICLES ========= */
const bg = document.getElementById('bg'), bgCtx = bg.getContext('2d');
let parts = [];
function rbg(){bg.width=innerWidth*devicePixelRatio;bg.height=innerHeight*devicePixelRatio;bg.style.width=innerWidth+'px';bg.style.height=innerHeight+'px';bgCtx.scale(devicePixelRatio,devicePixelRatio);initParts()}
function initParts(){parts=[];const n=Math.min(40,Math.floor(innerWidth/20));for(let i=0;i<n;i++)parts.push({x:Math.random()*innerWidth,y:Math.random()*innerHeight,vx:(Math.random()-.5)*.3,vy:(Math.random()-.5)*.3,r:Math.random()*1.5+.5,h:Math.random()*60+260})}
function drawBg(){bgCtx.clearRect(0,0,innerWidth,innerHeight);for(const p of parts){p.x+=p.vx;p.y+=p.vy;if(p.x<0||p.x>innerWidth)p.vx*=-1;if(p.y<0||p.y>innerHeight)p.vy*=-1;bgCtx.fillStyle=`hsla(${p.h},80%,70%,.5)`;bgCtx.beginPath();bgCtx.arc(p.x,p.y,p.r,0,7);bgCtx.fill()}for(let i=0;i<parts.length;i++)for(let j=i+1;j<parts.length;j++){const a=parts[i],b=parts[j],d=Math.hypot(a.x-b.x,a.y-b.y);if(d<120){bgCtx.strokeStyle=`hsla(280,60%,70%,${(1-d/120)*.08})`;bgCtx.lineWidth=.5;bgCtx.beginPath();bgCtx.moveTo(a.x,a.y);bgCtx.lineTo(b.x,b.y);bgCtx.stroke()}}requestAnimationFrame(drawBg)}
addEventListener('resize',rbg);rbg();drawBg();

/* ========= FLOW ========= */
function show(id){document.querySelectorAll('.screen').forEach(s=>s.classList.add('hidden'));document.getElementById(id).classList.remove('hidden');scrollTo(0,0)}
function vibe(){try{navigator.vibrate&&navigator.vibrate(15)}catch(e){}}

function start(){ans=[];qi=0;renderQ()}
function renderQ(){
	show('s-q');
	const q=Q[qi];
	document.getElementById('qnum').textContent=`QUESTION ${String(qi+1).padStart(2,'0')} / 12`;
	document.getElementById('qemoji').textContent=q.e;
	document.getElementById('qtext').textContent=q.t;
	const prog=document.getElementById('prog');prog.innerHTML='';for(let i=0;i<12;i++){const s=document.createElement('span');if(i<qi)s.className='done';else if(i===qi)s.className='cur';prog.appendChild(s)}
	const o=document.getElementById('opts');o.innerHTML='';
	['a','b'].forEach((k,i)=>{const b=document.createElement('button');b.className='opt';b.innerHTML=`<span class="mark">${'AB'[i]}</span><span>${q[k].t}</span>`;b.onclick=()=>pick(k);o.appendChild(b)})
}
function pick(k){vibe();const q=Q[qi];ans.push({dim:q.dim,val:q[k].d});document.querySelectorAll('.opt')[k==='a'?0:1].classList.add('pick');setTimeout(()=>{qi++;if(qi<Q.length)renderQ();else doLoad()},220)}

function doLoad(){
	show('s-load');
	const log=document.getElementById('loadlog');log.innerHTML='';let i=0;
	const t=setInterval(()=>{if(i>=LOAD_LOGS.length){clearInterval(t);setTimeout(showResult,400);return}const l=LOAD_LOGS[i];const line=document.createElement('div');line.innerHTML=l.startsWith('✓')?`<b class="ok">${l}</b>`:`<b>></b> ${l}`;log.appendChild(line);log.scrollTop=log.scrollHeight;i++},280)
}

function compute(){
	const s={M:0,A:0,H:0,D:0,S:0,T:0,O:0,C:0};
	ans.forEach(a=>{s[a.val]++});
	// egg detect: all 12 extremes — we consider every answer chose the second option
	const code=(s.M>=s.A?'M':'A')+(s.H>=s.D?'H':'D')+(s.S>=s.T?'S':'T')+(s.O>=s.C?'O':'C');
	return {code,s}
}

function showResult(codeOverride){
	const {code}= codeOverride?{code:codeOverride}:compute();
	let p = P[code];
	let isEgg=false;
	if(codeOverride && EGGS[codeOverride]){p=EGGS[codeOverride];isEgg=true}
	location.hash='#'+code;
	render(code,p,isEgg)
}

function render(code,p,isEgg){
	show('s-result');
	const root=document.getElementById('s-result');
	root.style.setProperty('--c1',p.c1);root.style.setProperty('--c2',p.c2);
	root.classList.add('result');
	const camp = code[0]==='M'?'模型派 · MODEL':'应用派 · APPLICATION';
	const count = bumpCount(code);
	root.innerHTML=`
		<div class="rhead">
			<div class="brand"><span class="dot"></span>YOUR AI PERSONA · 2026</div>
			<div class="rcode" data-code="${code}">${code}</div>
			<div class="rname">${p.n}</div>
			<div class="ren">${p.en}</div>
			<div class="rtag">${camp}</div>
		</div>
		${isEgg?`<div class="sec" style="background:linear-gradient(135deg,rgba(251,191,36,.1),rgba(245,158,11,.1));border-color:rgba(251,191,36,.3)"><span class="egg">HIDDEN</span><h3>🥚 隐藏人格</h3><p>你触发了极端答题路径，解锁了 16 型之外的第 17 种 AI 人格。这种人在 AI 圈极其稀少——你确定这真的是你？</p></div>`:''}
		<div class="sec"><h3><span class="e">🎭</span>人设 · IDENTITY</h3><p class="serif" style="font-style:italic;font-size:17px;color:#f0abfc;margin-bottom:12px">「${p.tag}」</p><p>${p.desc}</p></div>
		<div class="sec"><h3><span class="e">🧠</span>你的真实处境 · REALITY</h3><p>${p.real}</p></div>
		<div class="sec"><h3><span class="e">👯</span>你的队友 & 宿敌 · ALLIES</h3>
			<div class="pair">
				<div class="box good"><div class="lbl">&gt; BEST_MATCH</div><div class="val">${p.mateN}</div><div class="code">${p.mate}</div></div>
				<div class="box bad"><div class="lbl">&gt; NEMESIS</div><div class="val">${p.foeN}</div><div class="code">${p.foe}</div></div>
			</div>
			<p style="margin-top:12px;font-size:13px;color:var(--muted)">点击代号跳转到他们的人格页 →</p>
			<div class="btn-row" style="margin-top:8px">
				<button class="btn btn-ghost" style="font-size:13px;padding:10px" onclick="showResult('${p.mate}')">查看队友</button>
				<button class="btn btn-ghost" style="font-size:13px;padding:10px" onclick="showResult('${p.foe}')">查看宿敌</button>
			</div>
		</div>
		<div class="sec death"><h3><span class="e">⚰️</span>你会死于什么 · CAUSE OF DEATH</h3><p class="serif" style="font-size:16px">${p.death}</p></div>
		<div class="sec next"><h3><span class="e">🚀</span>你的下一步 · NEXT MOVE</h3><p style="font-size:16px;font-weight:500">${p.next}</p></div>
		<div class="sec" style="background:rgba(139,92,246,.06);border-color:rgba(139,92,246,.2)"><h3><span class="e">🪪</span>你的炫耀文案 · BRAG KIT</h3>
			<p style="font-size:13px;color:var(--muted);margin-bottom:10px">一键复制，粘贴到朋友圈/X/小红书简介</p>
			<div class="brag" id="brag">我是 ${code} · ${p.n}\n「${p.tag}」\n\n测你是 AI 时代的什么人 →\n${location.origin}${location.pathname}#${code}</div>
			<button class="btn btn-ghost" onclick="copyBrag()">📋 复制炫耀文案</button>
		</div>
		<div class="counter">已有 <b>${count.toLocaleString()}</b> 人发现自己是 <b>${code}</b></div>
		<div class="share-bar">
			<div class="btn-row">
				<button class="btn btn-primary" onclick="openShare('${code}')">🎨 生成分享海报</button>
			</div>
			<div class="btn-row">
				<button class="btn btn-ghost" onclick="openCompare()">⚔️ 对比朋友</button>
				<button class="btn btn-ghost" onclick="start()">🔁 重测</button>
			</div>
			<div class="footer-hint">把代号发给 3 个朋友，看看你们是队友还是宿敌</div>
		</div>
	`;
}

/* counter */
function bumpCount(code){
	const k='aipersona_count_'+code;
	const base={MHSC:2847,MHTC:1934,MHSO:4521,MHTO:2103,MDSC:1246,MDTC:893,MDSO:3654,MDTO:1568,AHSC:8934,AHTC:7621,AHSO:5412,AHTO:6783,ADSC:2341,ADTC:3892,ADSO:9823,ADTO:4267,VC:156,FOG:3241}[code]||1000;
	let c=+localStorage.getItem(k)||0;
	if(!sessionStorage.getItem('bumped_'+code)){c++;localStorage.setItem(k,c);sessionStorage.setItem('bumped_'+code,'1')}
	return base+c
}

/* brag copy */
function copyBrag(){const t=document.getElementById('brag').textContent;navigator.clipboard.writeText(t).then(()=>toast('已复制，去粘贴吧 🎉')).catch(()=>toast('请手动长按复制'))}

/* toast */
function toast(t){const el=document.createElement('div');el.className='toast';el.textContent=t;document.body.appendChild(el);setTimeout(()=>el.remove(),2100)}

/* ========= SHARE POSTER ========= */
function openShare(code){
	const p = P[code]||EGGS[code];if(!p)return;
	const m=document.createElement('div');m.className='modal';m.onclick=e=>{if(e.target===m)m.remove()};
	m.innerHTML=`<div class="card"><h4>🎨 你的专属海报</h4><canvas id="pcv" width="900" height="1600"></canvas><div class="tip">长按图片保存 / 截图分享到小红书、微信、X</div><div class="copyln"><span id="plink">${location.origin}${location.pathname}#${code}</span><button onclick="copyLink('${code}')">复制链接</button></div><button class="btn btn-ghost" onclick="this.closest('.modal').remove()">关闭</button></div>`;
	document.body.appendChild(m);
	drawPoster(code,p);
}
function copyLink(code){navigator.clipboard.writeText(location.origin+location.pathname+'#'+code).then(()=>toast('链接已复制'))}

function drawPoster(code,p){
	const c=document.getElementById('pcv'),g=c.getContext('2d'),W=900,H=1600;
	// bg gradient
	const grad=g.createLinearGradient(0,0,W,H);grad.addColorStop(0,'#0a0a12');grad.addColorStop(1,'#1a1030');g.fillStyle=grad;g.fillRect(0,0,W,H);
	// accent gradient blob
	const rg=g.createRadialGradient(W/2,H*.35,0,W/2,H*.35,700);rg.addColorStop(0,p.c1+'60');rg.addColorStop(1,'transparent');g.fillStyle=rg;g.fillRect(0,0,W,H);
	// grid
	g.strokeStyle='rgba(255,255,255,.04)';g.lineWidth=1;for(let x=0;x<W;x+=60){g.beginPath();g.moveTo(x,0);g.lineTo(x,H);g.stroke()}for(let y=0;y<H;y+=60){g.beginPath();g.moveTo(0,y);g.lineTo(W,y);g.stroke()}
	// top label
	g.fillStyle='rgba(255,255,255,.5)';g.font='600 22px "SF Mono",monospace';g.fillText('AI · PERSONA · TEST · 2026',60,90);
	g.fillStyle=p.c1;g.fillRect(60,110,40,3);
	// code mega
	const cg=g.createLinearGradient(0,250,0,500);cg.addColorStop(0,p.c1);cg.addColorStop(1,p.c2);g.fillStyle=cg;g.font='900 240px "SF Mono",monospace';g.textAlign='center';g.fillText(code,W/2,480);
	// name
	g.textAlign='center';g.fillStyle='#ffffff';g.font='800 72px "PingFang SC",sans-serif';g.fillText(p.n,W/2,610);
	// en
	g.fillStyle='rgba(255,255,255,.5)';g.font='500 26px "SF Mono",monospace';g.fillText(p.en.toUpperCase(),W/2,660);
	// tagline box
	g.fillStyle='rgba(255,255,255,.04)';roundRect(g,60,760,W-120,200,24);g.fill();g.strokeStyle='rgba(255,255,255,.1)';g.stroke();
	g.fillStyle=p.c1;g.font='italic 38px Georgia,"Songti SC",serif';wrap(g,'「'+p.tag+'」',W/2,835,W-180,52,true);
	// sections mini
	g.textAlign='left';g.fillStyle='rgba(255,255,255,.5)';g.font='600 22px "SF Mono",monospace';g.fillText('⚰ 你会死于:',60,1050);
	g.fillStyle='#fecaca';g.font='500 32px "PingFang SC",sans-serif';wrap(g,p.death,60,1100,W-120,44);
	g.fillStyle='rgba(255,255,255,.5)';g.font='600 22px "SF Mono",monospace';g.fillText('🚀 你的下一步:',60,1260);
	g.fillStyle='#bef264';g.font='500 32px "PingFang SC",sans-serif';wrap(g,p.next,60,1310,W-120,44);
	// footer
	g.fillStyle='rgba(255,255,255,.3)';g.font='500 22px "SF Mono",monospace';
	g.fillText('你是 AI 时代的什么人？',60,1480);
	g.fillStyle='#ffffff';g.font='700 28px "PingFang SC",sans-serif';
	g.fillText('测你是哪种 AI 物种 →',60,1520);
	g.fillStyle=p.c1;g.font='500 22px "SF Mono",monospace';
	const u=location.host+location.pathname+'#'+code;
	g.fillText(u.length>40?u.slice(0,40)+'...':u,60,1555);
}
function roundRect(g,x,y,w,h,r){g.beginPath();g.moveTo(x+r,y);g.arcTo(x+w,y,x+w,y+h,r);g.arcTo(x+w,y+h,x,y+h,r);g.arcTo(x,y+h,x,y,r);g.arcTo(x,y,x+w,y,r);g.closePath()}
function wrap(g,text,x,y,maxW,lh,center){const words=text.split('');let line='',lines=[];for(let i=0;i<words.length;i++){const tst=line+words[i];if(g.measureText(tst).width>maxW&&line.length){lines.push(line);line=words[i]}else line=tst}lines.push(line);lines.forEach((l,i)=>{g.textAlign=center?'center':'left';g.fillText(l,x,y+i*lh)})}

/* ========= COMPARE ========= */
function openCompare(){
	const myCode = location.hash.slice(1);
	const m=document.createElement('div');m.className='modal';m.onclick=e=>{if(e.target===m)m.remove()};
	m.innerHTML=`<div class="card"><h4>⚔️ 和朋友对比</h4><p class="tip">输入你朋友的 4 位代号（比如 ADSO），看你们是队友还是宿敌</p><input class="compare-input" id="cin" maxlength="4" placeholder="ABCD" autocomplete="off"/><button class="btn btn-primary" onclick="doCompare('${myCode}')">生成关系分析</button><div id="crel"></div><button class="btn btn-ghost" style="margin-top:14px" onclick="this.closest('.modal').remove()">关闭</button></div>`;
	document.body.appendChild(m);
	setTimeout(()=>document.getElementById('cin').focus(),100);
}
function doCompare(my){
	const other=document.getElementById('cin').value.toUpperCase().trim();
	if(!P[other]&&!EGGS[other]){toast('代号不存在，再确认一下');return}
	const mp=P[my]||EGGS[my], op=P[other]||EGGS[other];
	if(!mp){toast('你还没测试');return}
	// compute distance
	let same=0;for(let i=0;i<4;i++)if(my[i]===other[i])same++;
	let verdict,detail;
	if(my===other){verdict='👯 克隆体';detail='你们是同一物种。要么一起起飞，要么互相看不顺眼到分家。'}
	else if(same===3){verdict='💞 黄金搭档';detail='你们在一个维度上完美互补，其他都对齐。这是最稳的联创结构。'}
	else if(same===2){verdict='🤝 可共事';detail='有分歧但能互相补位，适合短期项目合作。长期要看价值观。'}
	else if(same===1){verdict='⚔️ 慢性宿敌';detail='你们会互相欣赏对方的才华，但每次决策都会吵架。最好不要合伙。'}
	else{verdict='☄️ 天敌';detail='你们的世界观完全对立，见面 5 分钟就能吵起来。但如果能合作，会是互联网奇迹。'}
	document.getElementById('crel').innerHTML=`<div class="relation"><div class="v">${verdict}</div><div class="d"><b style="color:${mp.c1}">${my}</b> × <b style="color:${op.c1}">${other}</b>（4 个维度中有 ${same} 个相同）<br><br>${detail}</div></div>`;
}

/* ========= HASH ROUTING ========= */
function checkHash(){
	const h=location.hash.slice(1).toUpperCase();
	if(h && (P[h]||EGGS[h])){
		showResult(h);return true;
	}
	return false;
}
addEventListener('hashchange',()=>{const h=location.hash.slice(1).toUpperCase();if(h&&(P[h]||EGGS[h])){showResult(h)}});
if(!checkHash())show('s-intro');

/* ========= EGG DETECTION OVERRIDE ========= */
// Hook into pick to detect egg path
const origPick = pick;
// easter egg: all answers match the 'b' option for 12 rounds (extreme path = VC observer)
// We'll detect based on pattern at compute time.
(function(){
	const _compute=compute;
	window.compute=function(){
		const base=_compute();
		// if user picked all 'b' (every answer maps to second pole) -> VC observer egg
		// Check if answers form pattern: M + D + S + C (all 'conservative') => egg VC
		const s=base.s;
		if(s.M>=3 && s.D>=3 && s.S>=3 && s.C>=3) return {code:'VC', egg:true};
		return base;
	};
	const _showResult = showResult;
	window.showResult=function(override){
		if(override){return _showResult(override)}
		const r=compute();
		if(r.egg){return _showResult(r.code)}
		return _showResult(r.code);
	}
})();
</script>
</body>
</html>
