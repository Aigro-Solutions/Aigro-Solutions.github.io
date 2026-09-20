* { box-sizing: border-box; }
:root {
  --bg-deep: #0a0d1a;
  --bg-panel: #10162c;
  --ink: #eef4ff;
  --muted: #b9c4dd;
  --gold: #f3d98a;
  --gold-strong: #e4b75d;
  --cyan: #7ee7ff;
  --purple: #8f7cff;
  --line: rgba(255, 255, 255, 0.12);
}
html { scroll-behavior: smooth; }
body {
  margin: 0;
  background: radial-gradient(circle at top, rgba(137, 92, 255, 0.2), transparent 20%), linear-gradient(180deg, #090d16 0%, #0c1120 100%);
  color: var(--ink);
  font-family: 'Inter', sans-serif;
}
a { color: inherit; text-decoration: none; }
.topbar {
  position: sticky; top: 0; z-index: 20;
  display: flex; justify-content: space-between; align-items: center;
  padding: 18px 7vw; backdrop-filter: blur(12px);
  background: rgba(8, 12, 20, 0.7); border-bottom: 1px solid var(--line);
}
.brand-wrap { display: flex; align-items: center; gap: 12px; }
.brand-mark {
  width: 36px; height: 36px; border-radius: 12px; display: grid; place-items: center;
  background: linear-gradient(135deg, var(--gold), var(--gold-strong)); color: #121827; font-weight: 800;
}
.brand-name { font-size: 0.82rem; letter-spacing: 0.16em; font-weight: 700; }
.brand-sub { font-size: 0.72rem; letter-spacing: 0.2em; opacity: 0.8; }
.nav { display: flex; gap: 22px; align-items: center; font-size: 0.88rem; color: var(--muted); }
.nav a:hover { color: var(--gold); }
.lang-switch {
  display: flex; align-items: center; gap: 10px; border: 1px solid var(--line); padding: 6px 10px; border-radius: 999px; background: rgba(255,255,255,0.02);
}
.lang-switch a { opacity: 0.75; font-size: 0.75rem; }
.lang-switch a.active { opacity: 1; color: var(--gold); }
.hero {
  display: grid; grid-template-columns: 1.1fr 0.9fr; max-width: 1200px; margin: 0 auto; padding: 80px 7vw 50px; gap: 32px; align-items: center;
}
.eyebrow { font-size: 0.8rem; letter-spacing: 0.28em; text-transform: uppercase; color: var(--gold); margin-bottom: 18px; }
.hero h1, .section-head h2, .book-cover h3, .book-cover h4, .hero-card h2 { font-family: 'Cormorant Garamond', serif; }
.hero h1 {
  margin: 0; font-size: clamp(3.5rem, 6vw, 7.2rem); line-height: 0.9; letter-spacing: -0.05em; color: var(--gold);
}
.subtitle { margin-top: 14px; font-size: clamp(1.1rem, 2vw, 1.8rem); color: #f7e9ba; letter-spacing: 0.08em; }
.lede { margin-top: 24px; max-width: 560px; font-size: 1.12rem; line-height: 1.8; color: var(--muted); }
.cta-row { margin-top: 30px; display: flex; gap: 16px; flex-wrap: wrap; }
.button { display: inline-flex; align-items: center; justify-content: center; padding: 14px 22px; border-radius: 999px; border: 1px solid transparent; font-weight: 700; transition: 0.2s ease; }
.button.primary { background: linear-gradient(135deg, var(--gold), var(--gold-strong)); color: #111827; }
.button.ghost { border-color: rgba(255,255,255,0.16); color: var(--ink); background: rgba(255,255,255,0.03); }
.button:hover { transform: translateY(-1px); }
.hero-card, .card, .manifesto-box, .contact-box, .book-cover, .book-copy { border: 1px solid var(--line); background: rgba(17, 22, 36, 0.7); border-radius: 22px; box-shadow: 0 18px 60px rgba(0,0,0,0.2); }
.hero-card { padding: 28px 24px; }
.mini-label { font-size: 0.72rem; letter-spacing: 0.2em; text-transform: uppercase; color: var(--gold); }
.hero-card h2 { margin: 18px 0 10px; font-size: 2.5rem; line-height: 1; }
.hero-card p, .hero-card li, .card p, .book-copy p, .manifesto-box p, .contact-box p { color: var(--muted); line-height: 1.7; }
.hero-card ul, .book-copy ul { margin: 18px 0 0; padding-left: 18px; color: var(--ink); }
.section { max-width: 1200px; margin: 0 auto; padding: 60px 7vw; }
.section.alt { background: rgba(255,255,255,0.015); border-top: 1px solid var(--line); border-bottom: 1px solid var(--line); }
.section-head { margin-bottom: 28px; }
.section-head h2 { margin: 0; font-size: clamp(2.4rem, 4vw, 4rem); line-height: 1; }
.grid.three { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 22px; }
.card { padding: 24px; }
.card-tag { display: inline-block; width: 42px; height: 42px; border-radius: 12px; display: grid; place-items: center; font-size: 0.8rem; color: #111827; background: linear-gradient(135deg, var(--gold), var(--gold-strong)); font-weight: 800; }
.card h3 { margin-top: 18px; margin-bottom: 12px; font-size: 1.6rem; }
.book-layout { display: grid; grid-template-columns: 0.7fr 1.3fr; gap: 28px; align-items: stretch; }
.book-cover {
  min-height: 340px; background: linear-gradient(180deg, rgba(15, 20, 37, 0.9), rgba(50, 34, 20, 0.75)); display: flex; flex-direction: column; justify-content: center; padding: 30px 24px;
}
.cover-badge { border: 1px solid rgba(255,255,255,0.18); border-radius: 999px; padding: 8px 12px; display: inline-block; font-size: 0.74rem; letter-spacing: 0.12em; text-transform: uppercase; color: var(--gold); width: fit-content; }
.book-cover h3, .book-cover h4 { margin: 18px 0 0; font-size: clamp(2.6rem, 4vw, 4.2rem); line-height: 0.9; color: var(--gold); }
.book-cover h4 { margin-top: 6px; }
.book-cover p { margin-top: 20px; color: var(--muted); line-height: 1.7; }
.book-copy { padding: 28px 26px; }
.manifesto-box { padding: 26px 24px; }
.contact-box { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 20px; padding: 30px 24px; }
.footer { border-top: 1px solid var(--line); text-align: center; padding: 30px 20px 50px; color: var(--muted); }
.page-shell { max-width: 1000px; margin: 0 auto; padding: 64px 24px 100px; }
.page-shell h1 { font-family: 'Cormorant Garamond', serif; font-size: clamp(3rem, 6vw, 5rem); color: var(--gold); margin: 0 0 16px; }
.page-shell p, .page-shell li { color: var(--muted); line-height: 1.8; }
.page-shell .body-block { background: rgba(255,255,255,0.02); border: 1px solid var(--line); border-radius: 22px; padding: 26px 22px; }
.page-shell .meta { margin-bottom: 28px; color: var(--gold); letter-spacing: 0.12em; text-transform: uppercase; font-size: 0.75rem; }
@media (max-width: 860px) {
  .topbar { flex-wrap: wrap; gap: 12px; }
  .nav { width: 100%; justify-content: center; flex-wrap: wrap; }
  .hero, .book-layout, .grid.three, .contact-box { grid-template-columns: 1fr; }
  .hero { padding-top: 40px; }
}
