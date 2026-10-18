<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Simple Farming Game</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@500;600;700&family=Inter:wght@400;500;600&family=Merriweather:wght@400;700&family=Luckiest+Guy&display=swap');

  :root {
    --sky-top: #bfe6f5;
    --sky-bottom: #eaf7ec;
    --soil: #8a5a3b;
    --soil-dark: #6e4529;
    --leaf: #4f9d5a;
    --leaf-dark: #397743;
    --sun: #ffc857;
    --card: #ffffff;
    --ink: #2f3b2d;
    --ink-soft: #6b7a68;
    --border: #d8e6d3;
    --ui-heading-font: 'Fredoka', sans-serif;
    --ui-body-font: 'Inter', sans-serif;
  }

  * { box-sizing: border-box; }

  body {
    margin: 0;
    min-height: 100vh;
    font-family: var(--ui-body-font);
    color: var(--ink);
    background: linear-gradient(180deg, var(--sky-top) 0%, var(--sky-bottom) 55%, #dff0d8 55%, #dff0d8 100%);
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    display: flex;
    justify-content: center;
    padding: 32px 16px;
    transition: background-image 0.3s ease;
  }

  .bg-picker {
    display: flex;
    align-items: center;
    gap: 8px;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 999px;
    padding: 6px 8px 6px 16px;
    box-shadow: 0 2px 0 var(--border);
    font-size: 13px;
    font-weight: 500;
    color: var(--ink-soft);
  }

  .bg-picker button {
    font-family: var(--ui-body-font);
    font-size: 12px;
    font-weight: 600;
    padding: 6px 12px;
    border-radius: 999px;
    border: 1px solid var(--border);
    background: #fbfdf9;
    cursor: pointer;
    color: var(--ink);
  }

  .bg-picker button:hover { background: #f1f9ee; border-color: var(--leaf); }
  .bg-picker input[type="file"] { display: none; }

  .app {
    width: 100%;
    max-width: 760px;
  }

  header {
    display: flex;
    align-items: baseline;
    justify-content: space-between;
    margin-bottom: 18px;
    flex-wrap: wrap;
    gap: 8px;
  }

  h1 {
    font-family: var(--ui-heading-font);
    font-size: 32px;
    font-weight: 700;
    margin: 0;
    color: var(--leaf-dark);
    letter-spacing: -0.5px;
  }

  .weather-badge {
    font-family: var(--ui-heading-font);
    font-size: 14px;
    font-weight: 600;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 999px;
    padding: 6px 14px;
    box-shadow: 0 2px 0 var(--border);
    color: var(--ink-soft);
    white-space: nowrap;
  }

  .xp-badge {
    display: flex;
    align-items: center;
    gap: 8px;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 999px;
    padding: 6px 14px;
    box-shadow: 0 2px 0 var(--border);
  }

  .xp-badge-level {
    font-family: var(--ui-heading-font);
    font-size: 13px;
    font-weight: 700;
    color: var(--leaf-dark);
    white-space: nowrap;
  }

  .xp-badge-track {
    width: 64px;
    height: 6px;
    border-radius: 4px;
    background: var(--border);
    overflow: hidden;
  }

  .xp-badge-fill {
    height: 100%;
    width: 0%;
    background: linear-gradient(90deg, var(--sun), #ffe08a);
    transition: width 0.3s ease;
  }

  .wallet {
    font-family: var(--ui-heading-font);
    font-size: 20px;
    font-weight: 600;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 999px;
    padding: 8px 18px;
    box-shadow: 0 2px 0 var(--border);
  }

  .panel {
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 18px;
    padding: 18px;
    margin-bottom: 18px;
    box-shadow: 0 3px 0 var(--border);
  }

  .panel h2 {
    font-family: var(--ui-heading-font);
    font-size: 15px;
    text-transform: uppercase;
    letter-spacing: 0.08em;
    color: var(--ink-soft);
    margin: 0 0 12px 0;
  }

  .seed-shelf {
    display: flex;
    gap: 8px;
    flex-wrap: nowrap;
    overflow-x: auto;
    padding-bottom: 6px;
    scrollbar-width: thin;
    scrollbar-color: var(--leaf) #eef4ea;
  }

  .seed-shelf::-webkit-scrollbar { height: 6px; }
  .seed-shelf::-webkit-scrollbar-track { background: #eef4ea; border-radius: 4px; }
  .seed-shelf::-webkit-scrollbar-thumb { background: var(--leaf); border-radius: 4px; }

  .seed-card {
    flex: 0 0 96px;
    border: 2px solid var(--border);
    border-radius: 12px;
    padding: 8px 6px;
    background: #fbfdf9;
    cursor: pointer;
    transition: transform 0.12s ease, border-color 0.12s ease;
    text-align: center;
    font-family: var(--ui-body-font);
    position: relative;
  }

  .seed-card:hover { transform: translateY(-2px); }
  .seed-card.selected {
    border-color: var(--leaf);
    background: #f1f9ee;
  }

  .seed-card.locked {
    cursor: default;
    opacity: 0.55;
    background: #f2f2ee;
  }
  .seed-card.locked:hover { transform: none; }
  .seed-card.locked .emoji { filter: grayscale(1); }

  /* Locked rebirth-exclusive crops look chained up — dashed purple border, chain-link
     emoji clamps top and bottom, and a slow rattle to suggest they're straining against it. */
  .seed-card.locked.rebirth-locked {
    position: relative;
    border-style: dashed;
    border-color: #9b59d0;
    background: repeating-linear-gradient(135deg, #f5edfb, #f5edfb 8px, #ecdcf9 8px, #ecdcf9 16px);
    opacity: 0.75;
    animation: chain-rattle 3.4s ease-in-out infinite;
  }

  .seed-card.locked.rebirth-locked::before,
  .seed-card.locked.rebirth-locked::after {
    content: '⛓️';
    position: absolute;
    left: 50%;
    font-size: 13px;
    filter: drop-shadow(0 0 2px rgba(155, 89, 208, 0.6));
  }
  .seed-card.locked.rebirth-locked::before {
    top: -9px;
    transform: translateX(-50%) rotate(-10deg);
  }
  .seed-card.locked.rebirth-locked::after {
    bottom: -9px;
    transform: translateX(-50%) rotate(10deg);
  }

  @keyframes chain-rattle {
    0%, 100% { transform: rotate(0deg); }
    25% { transform: rotate(-1.2deg); }
    75% { transform: rotate(1.2deg); }
  }

  .seed-card.rebirth-exclusive {
    border-color: #9b59d0;
    background: linear-gradient(180deg, #faf5ff, #f0e4fb);
  }

  .rebirth-exclusive-tag {
    font-size: 9px;
    font-weight: 700;
    color: #7c3fa6;
    background: #ecdcf9;
    border-radius: 999px;
    padding: 2px 6px;
    display: inline-block;
    margin-bottom: 2px;
  }

  /* Plays once, right when a rebirth pushes a crop's rebirthRequired threshold past —
     the chains visually shatter with a purple flash and a bounce. */
  .seed-card.chain-break {
    animation: chain-break-burst 1.1s ease-out;
  }

  @keyframes chain-break-burst {
    0% { transform: scale(1); box-shadow: none; }
    25% { transform: scale(1.18) rotate(-2deg); box-shadow: 0 0 0 6px rgba(155, 89, 208, 0.45), 0 0 24px 10px rgba(155, 89, 208, 0.6); }
    55% { transform: scale(1.08) rotate(2deg); box-shadow: 0 0 0 4px rgba(155, 89, 208, 0.3), 0 0 16px 6px rgba(155, 89, 208, 0.4); }
    100% { transform: scale(1) rotate(0deg); box-shadow: none; }
  }

  @media (prefers-reduced-motion: reduce) {
    .seed-card.locked.rebirth-locked, .seed-card.chain-break { animation: none; }
  }


  .seed-card .emoji { font-size: 22px; }
  .seed-card .name { font-weight: 600; margin-top: 2px; font-size: 12px; }
  .seed-card .meta { font-size: 10px; color: var(--ink-soft); margin-top: 1px; line-height: 1.3; }
  .seed-card .owned {
    position: absolute;
    top: 5px;
    right: 6px;
    font-size: 10px;
    font-weight: 600;
    color: var(--leaf-dark);
  }

  .buy-row {
    display: flex;
    flex-direction: column;
    gap: 3px;
    margin-top: 6px;
  }

  .buy-row button {
    flex: 1;
    font-family: var(--ui-body-font);
    font-size: 10px;
    font-weight: 600;
    padding: 4px 2px;
    border-radius: 6px;
    border: 1px solid var(--border);
    background: #fff;
    cursor: pointer;
    color: var(--ink);
  }

  .buy-row button:hover { background: #f1f9ee; border-color: var(--leaf); }
  .buy-row button:disabled { opacity: 0.4; cursor: not-allowed; }

  .field {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(88px, 1fr));
    gap: 12px;
  }

  .plot {
    aspect-ratio: 1;
    border-radius: 16px;
    background: var(--soil);
    background-image:
      linear-gradient(180deg, rgba(0,0,0,0.05), transparent 40%),
      repeating-linear-gradient(115deg, rgba(0,0,0,0.06) 0 6px, transparent 6px 16px);
    border: 3px solid var(--soil-dark);
    position: relative;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
    transition: transform 0.1s ease;
  }

  .plot:active { transform: scale(0.97); }

  .plot .crop-emoji {
    position: relative;
    z-index: 1;
    font-size: 42px;
    filter: drop-shadow(0 3px 2px rgba(0,0,0,0.25));
    transition: transform 0.25s ease;
  }

  .plot.ready .crop-emoji {
    animation: bob 0.9s ease-in-out infinite;
  }

  @keyframes bob {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-6px); }
  }

  .plot .progress-track {
    position: absolute;
    z-index: 1;
    bottom: 8px;
    left: 8px;
    right: 8px;
    height: 6px;
    border-radius: 4px;
    background: rgba(0,0,0,0.25);
    overflow: hidden;
  }

  .plot .progress-fill {
    height: 100%;
    background: var(--sun);
    width: 0%;
    transition: width 0.3s linear;
  }

  .plot.ready .progress-fill { background: #7ee08a; }

  .plot .ready-badge {
    position: absolute;
    z-index: 1;
    top: 6px;
    right: 6px;
    background: #7ee08a;
    color: #1c3d1f;
    font-size: 11px;
    font-weight: 700;
    padding: 2px 7px;
    border-radius: 999px;
  }

  .plot .regrow-badge {
    position: absolute;
    z-index: 1;
    top: 6px;
    left: 6px;
    background: rgba(255,255,255,0.85);
    color: var(--ink);
    font-size: 10px;
    font-weight: 700;
    padding: 2px 6px;
    border-radius: 999px;
  }

  /* Mutation cue: a small badge showing every stacked mutation icon, plus a
     glowing border AND a colored background wash so the plot itself visibly
     changes depending on what it's growing. */
  .plot .mutation-hint {
    position: absolute;
    bottom: 8px;
    right: 8px;
    font-size: 15px;
    letter-spacing: 1px;
    filter: drop-shadow(0 0 3px rgba(255,255,255,0.9));
    animation: mutation-hint-pulse 1.6s ease-in-out infinite;
    z-index: 2;
  }

  @keyframes mutation-hint-pulse {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.2); }
  }

  .plot.mutating {
    position: relative;
    animation: mutation-glow 1.8s ease-in-out infinite;
  }

  .plot.mutating::before {
    content: '';
    position: absolute;
    inset: 0;
    border-radius: 13px;
    pointer-events: none;
    z-index: 0;
    background: var(--mutation-tint, transparent);
  }

  @keyframes mutation-glow {
    0%, 100% { box-shadow: 0 0 0 0 rgba(255, 200, 87, 0.5); }
    50% { box-shadow: 0 0 14px 4px rgba(255, 200, 87, 0.65); }
  }

  .plot.mutating.mutation-giant {
    --mutation-tint: rgba(143, 184, 230, 0.35);
  }

  .plot.mutating.mutation-golden {
    --mutation-tint: rgba(255, 200, 87, 0.4);
    animation-name: mutation-glow-golden;
  }
  @keyframes mutation-glow-golden {
    0%, 100% { box-shadow: 0 0 0 0 rgba(255, 200, 87, 0.55); }
    50% { box-shadow: 0 0 16px 5px rgba(255, 200, 87, 0.75); }
  }

  .plot.mutating.mutation-rainbow {
    --mutation-tint: linear-gradient(135deg, rgba(255,120,120,0.3), rgba(255,220,120,0.3), rgba(120,220,160,0.3), rgba(120,160,255,0.3), rgba(200,120,255,0.3));
    animation-name: mutation-glow-rainbow;
  }
  @keyframes mutation-glow-rainbow {
    0%   { box-shadow: 0 0 12px 4px rgba(255,120,120,0.55); }
    25%  { box-shadow: 0 0 12px 4px rgba(255,220,120,0.55); }
    50%  { box-shadow: 0 0 12px 4px rgba(120,220,160,0.55); }
    75%  { box-shadow: 0 0 12px 4px rgba(120,160,255,0.55); }
    100% { box-shadow: 0 0 12px 4px rgba(200,120,255,0.55); }
  }

  .plot.mutating.mutation-crystal {
    --mutation-tint: rgba(109, 214, 214, 0.35);
    animation-name: mutation-glow-crystal;
  }
  @keyframes mutation-glow-crystal {
    0%, 100% { box-shadow: 0 0 0 0 rgba(109, 214, 214, 0.55); }
    50% { box-shadow: 0 0 16px 5px rgba(109, 214, 214, 0.75); }
  }

  .plot.mutating.mutation-diamond {
    --mutation-tint: rgba(126, 168, 232, 0.4);
    animation-name: mutation-glow-diamond;
  }
  @keyframes mutation-glow-diamond {
    0%, 100% { box-shadow: 0 0 0 0 rgba(126, 168, 232, 0.6); }
    50% { box-shadow: 0 0 18px 6px rgba(126, 168, 232, 0.85); }
  }

  .plot.mutating.mutation-cosmic {
    --mutation-tint: rgba(155, 126, 232, 0.45);
    animation-name: mutation-glow-cosmic;
  }
  @keyframes mutation-glow-cosmic {
    0%, 100% { box-shadow: 0 0 0 0 rgba(155, 126, 232, 0.65); }
    50% { box-shadow: 0 0 20px 6px rgba(155, 126, 232, 0.9); }
  }

  .plot.mutating.mutation-celestial {
    --mutation-tint: rgba(255, 200, 87, 0.5);
    animation-name: mutation-glow-celestial;
  }
  @keyframes mutation-glow-celestial {
    0%, 100% { box-shadow: 0 0 0 0 rgba(255, 200, 87, 0.7); }
    50% { box-shadow: 0 0 22px 7px rgba(255, 200, 87, 0.95); }
  }

  .plot.mutating.mutation-voidtouched {
    --mutation-tint: rgba(74, 58, 107, 0.55);
    animation-name: mutation-glow-void;
  }
  @keyframes mutation-glow-void {
    0%, 100% { box-shadow: 0 0 0 0 rgba(74, 58, 107, 0.8); }
    50% { box-shadow: 0 0 26px 8px rgba(74, 58, 107, 1); }
  }

  @media (prefers-reduced-motion: reduce) {
    .plot.mutating, .plot .mutation-hint { animation: none; }
  }

  .plot .empty-hint {
    font-size: 12px;
    color: rgba(255,255,255,0.75);
    text-align: center;
    padding: 0 8px;
    font-family: var(--ui-body-font);
  }

  .toast {
    position: fixed;
    bottom: 22px;
    left: 50%;
    transform: translateX(-50%) translateY(20px);
    background: var(--ink);
    color: #fff;
    padding: 10px 20px;
    border-radius: 999px;
    font-size: 14px;
    font-weight: 500;
    opacity: 0;
    pointer-events: none;
    transition: opacity 0.25s ease, transform 0.25s ease;
  }

  .toast.show {
    opacity: 1;
    transform: translateX(-50%) translateY(0);
  }

  .hint {
    font-size: 13px;
    color: var(--ink-soft);
    margin: -6px 0 16px 2px;
  }

  .gear-armed-banner {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 10px;
    background: #fff3cd;
    border: 2px solid #f0b73f;
    border-radius: 12px;
    padding: 8px 12px;
    margin-bottom: 12px;
    font-size: 13px;
    font-weight: 600;
    color: #6b4a1f;
  }

  .gear-armed-banner button {
    font-family: var(--ui-body-font);
    font-size: 12px;
    font-weight: 600;
    padding: 4px 10px;
    border-radius: 8px;
    border: 1px solid #f0b73f;
    background: #fff;
    cursor: pointer;
    color: #6b4a1f;
  }

  @media (prefers-reduced-motion: reduce) {
    .plot.ready .crop-emoji { animation: none; }
  }

  .upgrades-tab {
    position: fixed;
    right: 0;
    top: 50%;
    transform: translateY(-50%);
    background: var(--leaf);
    color: #fff;
    border: none;
    border-radius: 12px 0 0 12px;
    padding: 14px 10px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 6px;
    font-size: 20px;
    cursor: pointer;
    box-shadow: -2px 2px 8px rgba(0,0,0,0.15);
    transition: padding 0.15s ease, background 0.15s ease;
  }

  .upgrades-tab.inventory-tab {
    top: calc(50% - 184px);
    background: var(--sun);
    color: #5c4108;
  }
  .upgrades-tab.inventory-tab:hover {
    background: #f0b73f;
  }

  .upgrades-tab.quests-tab {
    top: calc(50% - 92px);
    background: #b5762a;
    color: #fff;
  }
  .upgrades-tab.quests-tab:hover {
    background: #9c6323;
  }

  .upgrades-tab.gearshop-tab {
    top: 50%;
    background: #2e8b6f;
    color: #fff;
  }
  .upgrades-tab.gearshop-tab:hover {
    background: #26735c;
  }

  .upgrades-tab.gear-tab {
    top: calc(50% + 92px);
  }

  .upgrades-tab.rebirth-tab {
    top: calc(50% + 184px);
    background: #9b59d0;
    color: #fff;
  }
  .upgrades-tab.rebirth-tab:hover {
    background: #8347b8;
  }

  .tutorial-tab {
    position: fixed;
    left: 0;
    top: calc(50% - 46px);
    transform: translateY(-50%);
    background: #3fa7d6;
    color: #fff;
    border: none;
    border-radius: 0 12px 12px 0;
    padding: 14px 10px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 6px;
    font-size: 20px;
    cursor: pointer;
    box-shadow: 2px 2px 8px rgba(0,0,0,0.15);
    transition: padding 0.15s ease, background 0.15s ease;
    z-index: 40;
  }

  .tutorial-tab.settings-tab {
    top: calc(50% + 46px);
    background: #607d8b;
  }
  .tutorial-tab.settings-tab:hover {
    background: #4e6a76;
  }

  .tutorial-tab:hover {
    background: #2f8fb8;
    padding-left: 16px;
  }
  .tutorial-tab span {
    font-family: var(--ui-heading-font);
    font-size: 11px;
    font-weight: 600;
    writing-mode: vertical-rl;
    text-orientation: mixed;
    letter-spacing: 0.04em;
  }

  .tutorial-panel {
    position: fixed;
    left: 0;
    top: 0;
    bottom: 0;
    width: 300px;
    max-width: 85vw;
    background: var(--card);
    border-right: 1px solid var(--border);
    box-shadow: 4px 0 16px rgba(0,0,0,0.12);
    transform: translateX(-100%);
    transition: transform 0.25s ease;
    z-index: 45;
    display: flex;
    flex-direction: column;
  }
  .tutorial-panel.open {
    transform: translateX(0);
  }

  .tutorial-panel-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 18px 20px;
    border-bottom: 1px solid var(--border);
    flex: 0 0 auto;
  }
  .tutorial-panel-header h2 {
    font-family: var(--ui-heading-font);
    font-size: 20px;
    margin: 0;
    color: var(--leaf-dark);
  }

  .tutorial-panel-body {
    padding: 16px 20px 24px;
    overflow-y: auto;
    flex: 1 1 auto;
  }
  .tutorial-panel-body section {
    margin-bottom: 18px;
  }
  .tutorial-panel-body h3 {
    font-family: var(--ui-heading-font);
    font-size: 14px;
    margin: 0 0 4px;
    color: var(--ink);
  }
  .tutorial-panel-body p {
    font-size: 12.5px;
    line-height: 1.5;
    color: var(--ink-soft);
    margin: 0;
  }

  .settings-option-row {
    display: flex;
    flex-wrap: wrap;
    gap: 8px;
  }

  .settings-option-btn {
    font-family: var(--ui-body-font);
    font-size: 12px;
    font-weight: 600;
    padding: 8px 12px;
    border-radius: 10px;
    border: 1px solid var(--border);
    background: var(--card);
    color: var(--ink);
    cursor: pointer;
    transition: border-color 0.15s ease, background 0.15s ease;
  }
  .settings-option-btn:hover {
    border-color: var(--leaf);
  }
  .settings-option-btn.active {
    border-color: var(--leaf);
    background: var(--leaf);
    color: #fff;
  }

  /* Show/hide toggle for every side tab (left + right). The toggle button itself
     is never hidden by its own state — it's always reachable. */
  .upgrades-tab,
  .tutorial-tab {
    transition: opacity 0.2s ease, padding 0.15s ease, background 0.15s ease;
  }

  body.tabs-hidden .upgrades-tab,
  body.tabs-hidden .tutorial-tab {
    opacity: 0;
    pointer-events: none;
  }

  .tabs-toggle-btn {
    position: fixed;
    top: 14px;
    right: 14px;
    z-index: 50;
    width: 34px;
    height: 34px;
    border-radius: 50%;
    border: 1px solid var(--border);
    background: var(--card);
    box-shadow: 0 2px 0 var(--border);
    font-size: 15px;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .tabs-toggle-btn:hover {
    background: #f1f9ee;
  }

  .upgrades-tab span {
    font-family: var(--ui-heading-font);
    font-size: 11px;
    font-weight: 600;
    writing-mode: vertical-rl;
    text-orientation: mixed;
    letter-spacing: 0.04em;
  }

  .upgrades-tab:hover {
    background: var(--leaf-dark);
    padding-right: 16px;
  }

  .modal-backdrop {
    position: fixed;
    inset: 0;
    background: rgba(47, 59, 45, 0.45);
    display: none;
    align-items: center;
    justify-content: center;
    padding: 20px;
    z-index: 50;
  }

  .modal-backdrop.open { display: flex; }

  .modal {
    background: var(--card);
    border-radius: 20px;
    width: 100%;
    max-width: 460px;
    max-height: 82vh;
    display: flex;
    flex-direction: column;
    box-shadow: 0 12px 0 var(--border);
    border: 1px solid var(--border);
  }

  .modal-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 18px 20px;
    border-bottom: 1px solid var(--border);
  }

  .modal-header h2 {
    font-family: var(--ui-heading-font);
    font-size: 20px;
    margin: 0;
    color: var(--leaf-dark);
  }

  .modal-close {
    border: none;
    background: #f2f2ee;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    font-size: 14px;
    cursor: pointer;
    color: var(--ink-soft);
  }
  .modal-close:hover { background: #e6e6e0; }

  .modal-body {
    padding: 18px 20px 22px;
    overflow-y: auto;
    display: flex;
    flex-direction: column;
    gap: 12px;
  }

  .upgrade-card {
    border: 2px solid var(--border);
    border-radius: 14px;
    padding: 12px 14px;
    display: flex;
    align-items: center;
    gap: 12px;
  }

  .upgrade-card .icon {
    font-size: 26px;
    flex: 0 0 auto;
  }

  .upgrade-card .info { flex: 1; }
  .upgrade-card .info .name {
    font-weight: 600;
    font-size: 14px;
  }
  .upgrade-card .info .desc {
    font-size: 12px;
    color: var(--ink-soft);
    margin-top: 2px;
  }
  .upgrade-card .info .level {
    font-size: 11px;
    color: var(--leaf-dark);
    font-weight: 600;
    margin-top: 4px;
  }

  .upgrade-card button {
    flex: 0 0 auto;
    font-family: var(--ui-body-font);
    font-size: 12px;
    font-weight: 600;
    padding: 8px 12px;
    border-radius: 10px;
    border: 1px solid var(--border);
    background: #fbfdf9;
    cursor: pointer;
    white-space: nowrap;
  }
  .upgrade-card button:hover:not(:disabled) { background: #f1f9ee; border-color: var(--leaf); }
  .upgrade-card button:disabled { opacity: 0.45; cursor: not-allowed; }

  /* Quest board — parchment/scroll styling to feel like a physical quest board */
  .quest-card {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 14px;
    margin-bottom: 10px;
    border-radius: 12px;
    border: 2px solid #d8b877;
    background: linear-gradient(180deg, #fdf6e3, #f5e8c8);
    box-shadow: inset 0 0 0 1px rgba(180, 130, 50, 0.15), 0 2px 0 #cfa858;
  }

  .quest-card.done {
    border-color: var(--leaf);
    background: linear-gradient(180deg, #f1f9ee, #e3f5da);
    box-shadow: inset 0 0 0 1px rgba(79, 157, 90, 0.2), 0 2px 0 var(--leaf);
  }

  .quest-card .icon {
    font-size: 26px;
    flex: 0 0 auto;
  }

  .quest-card .info { flex: 1; min-width: 0; }

  .quest-card .name {
    font-family: var(--ui-heading-font);
    font-weight: 600;
    font-size: 14px;
    color: #6b4a1f;
    margin-bottom: 6px;
  }

  .quest-card.done .name { color: var(--leaf-dark); }

  .quest-progress-track {
    height: 8px;
    border-radius: 4px;
    background: rgba(180, 130, 50, 0.2);
    overflow: hidden;
    margin-bottom: 6px;
  }

  .quest-progress-fill {
    height: 100%;
    background: linear-gradient(90deg, #d8b877, var(--sun));
    transition: width 0.3s ease;
  }

  .quest-card.done .quest-progress-fill { background: var(--leaf); }

  .quest-card .desc {
    font-size: 11px;
    color: #8a6a3a;
  }

  .quest-card.done .desc { color: var(--ink-soft); }

  .quest-card button {
    flex: 0 0 auto;
    font-family: var(--ui-body-font);
    font-size: 12px;
    font-weight: 700;
    padding: 8px 14px;
    border-radius: 10px;
    border: none;
    background: var(--leaf);
    color: #fff;
    cursor: pointer;
  }
  .quest-card button:disabled {
    background: #d8b877;
    opacity: 0.6;
    cursor: not-allowed;
  }


  .upgrade-card.owned {
    border-color: var(--leaf);
    background: #f1f9ee;
  }

  .upgrade-card.locked {
    opacity: 0.55;
    background: #f2f2ee;
  }
  .upgrade-card.locked .icon { filter: grayscale(1); }

  .upgrade-card.mutation-giant { border-color: #8fb8e6; background: #f0f6fc; }
  .upgrade-card.mutation-golden { border-color: var(--sun); background: #fffbea; }
  .upgrade-card.mutation-rainbow {
    border-color: #d68fe6;
    background: linear-gradient(135deg, #fff0f0, #fff8e0, #f0fff4, #f0f4ff);
  }

  .upgrade-card.mutation-crystal {
    border-color: #6dd6d6;
    background: linear-gradient(135deg, #eafffe, #e0f7ff);
  }

  .upgrade-card.mutation-diamond {
    border-color: #7ea8e8;
    background: linear-gradient(135deg, #eef4ff, #e3edff);
    box-shadow: 0 0 0 2px rgba(126, 168, 232, 0.25);
  }

  .upgrade-card.mutation-cosmic {
    border-color: #9b7ee8;
    background: linear-gradient(135deg, #f3eeff, #2b1f4a);
    color: #fff;
  }
  .upgrade-card.mutation-cosmic .desc { color: #d8ccf7; }

  .upgrade-card.mutation-celestial {
    border-color: var(--sun);
    background: linear-gradient(135deg, #fff8e0, #ffe9a8);
    box-shadow: 0 0 0 3px rgba(255, 200, 87, 0.35);
  }

  .upgrade-card.mutation-voidtouched {
    border-color: #4a3a6b;
    background: linear-gradient(135deg, #1a1425, #3a2a5c);
    color: #e8ddff;
    box-shadow: 0 0 12px rgba(74, 58, 107, 0.6);
  }
  .upgrade-card.mutation-voidtouched .desc { color: #c4b0ec; }

  .tree-branch {
    display: flex;
    flex-direction: column;
    align-items: stretch;
    margin-top: 6px;
    padding-top: 12px;
    border-top: 1px dashed var(--border);
  }

  .tree-branch-title {
    font-family: var(--ui-heading-font);
    font-size: 13px;
    font-weight: 600;
    color: var(--ink-soft);
    text-transform: uppercase;
    letter-spacing: 0.06em;
    margin-bottom: 8px;
  }

  .skill-tree {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 6px 0 4px;
  }

  .tree-root-wrap { display: flex; justify-content: center; }

  .tree-connector-line {
    width: 2px;
    height: 16px;
    background: var(--border);
  }

  .tree-crossbar {
    width: 78%;
    max-width: 320px;
    height: 2px;
    background: var(--border);
  }

  .tree-stub {
    width: 2px;
    height: 16px;
    background: var(--border);
  }

  .tree-columns {
    display: flex;
    justify-content: center;
    gap: 22px;
    flex-wrap: wrap;
  }

  .tree-column {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 6px;
  }

  .tree-column-label {
    font-family: var(--ui-heading-font);
    font-size: 11px;
    font-weight: 600;
    color: var(--ink-soft);
    text-transform: uppercase;
    letter-spacing: 0.05em;
    margin-bottom: 2px;
    white-space: nowrap;
  }

  .tree-node-circle {
    position: relative;
    width: 56px;
    height: 56px;
    border-radius: 50%;
    border: 3px solid var(--border);
    background: #fbfdf9;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 24px;
    cursor: pointer;
    padding: 0;
    transition: transform 0.12s ease, border-color 0.12s ease;
  }

  .tree-node-circle:hover { transform: translateY(-2px); }

  .tree-node-circle.owned {
    border-color: var(--leaf);
    background: #eafbe9;
  }

  .tree-node-circle.available {
    border-color: var(--sun);
    box-shadow: 0 0 0 4px rgba(255, 200, 87, 0.28);
  }

  .tree-node-circle.locked {
    opacity: 0.5;
    filter: grayscale(1);
    cursor: not-allowed;
  }
  .tree-node-circle.locked:hover { transform: none; }

  .tree-node-circle.selected {
    outline: 3px solid var(--leaf-dark);
    outline-offset: 2px;
  }

  .tree-node-badge {
    position: absolute;
    bottom: -6px;
    right: -6px;
    background: var(--ink);
    color: #fff;
    font-size: 9px;
    font-weight: 700;
    padding: 2px 5px;
    border-radius: 999px;
    line-height: 1.3;
  }
  .tree-node-badge.check { background: var(--leaf-dark); }

  .tree-node-wrap {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 4px;
  }

  .tree-node-price {
    font-size: 11px;
    font-weight: 600;
    color: var(--ink-soft);
    white-space: nowrap;
  }

  .tree-detail {
    margin-top: 16px;
    padding-top: 14px;
    border-top: 1px dashed var(--border);
  }
</style>
</head>
<body>
<div class="app">
  <header>
    <h1>Simple Farming Game</h1>
    <div class="xp-badge" id="xpBadge">
      <span class="xp-badge-level">Lv 1</span>
      <div class="xp-badge-track"><div class="xp-badge-fill" id="xpBadgeFill"></div></div>
    </div>
    <div class="weather-badge" id="weatherBadge">☀️ Sunny</div>
    <div class="wallet" id="wallet">0 🪙</div>
  </header>

  <div class="bg-picker">
    <span>Background:</span>
    <button id="bgUploadBtn" type="button">Choose photo…</button>
    <button id="bgResetBtn" type="button">Reset</button>
    <input type="file" id="bgInput" accept="image/*">
  </div>
  <div style="height:14px"></div>

  <p class="hint">Pick a seed below, then tap an empty plot to plant it. Tap a glowing plot to harvest it into your 🎒 Inventory — sell it there whenever you like.</p>

  <div class="panel">
    <h2>Seed Shelf</h2>
    <div class="seed-shelf" id="seedShelf"></div>
  </div>

  <div class="panel">
    <h2>Your Field</h2>
    <div class="gear-armed-banner" id="gearArmedBanner" style="display:none;"></div>
    <div class="field" id="field"></div>
  </div>
</div>

<button class="upgrades-tab inventory-tab" id="inventoryBtn" type="button" title="Inventory">
  🎒<span>Inventory</span>
</button>

<div class="modal-backdrop" id="inventoryBackdrop">
  <div class="modal">
    <div class="modal-header">
      <h2>Inventory</h2>
      <button class="modal-close" id="inventoryCloseBtn" type="button" aria-label="Close">✕</button>
    </div>
    <div class="modal-body" id="inventoryList"></div>
  </div>
</div>

<button class="upgrades-tab quests-tab" id="questsBtn" type="button" title="Quests">
  📜<span>Quests</span>
</button>

<div class="modal-backdrop" id="questsBackdrop">
  <div class="modal">
    <div class="modal-header">
      <h2>Quest Board</h2>
      <button class="modal-close" id="questsCloseBtn" type="button" aria-label="Close">✕</button>
    </div>
    <div class="modal-body" id="questsList"></div>
  </div>
</div>

<button class="upgrades-tab gearshop-tab" id="gearShopBtn" type="button" title="Gear Shop">
  🧴<span>Gear Shop</span>
</button>

<div class="modal-backdrop" id="gearBackdrop">
  <div class="modal">
    <div class="modal-header">
      <h2>Gear Shop</h2>
      <button class="modal-close" id="gearCloseBtn" type="button" aria-label="Close">✕</button>
    </div>
    <div class="modal-body" id="gearShopList"></div>
  </div>
</div>

<button class="upgrades-tab gear-tab" id="upgradesBtn" type="button" title="Upgrades">
  🛠<span>Upgrades</span>
</button>

<div class="modal-backdrop" id="upgradesBackdrop">
  <div class="modal">
    <div class="modal-header">
      <h2>Farm Upgrades</h2>
      <button class="modal-close" id="upgradesCloseBtn" type="button" aria-label="Close">✕</button>
    </div>
    <div class="modal-body" id="upgradesList"></div>
  </div>
</div>

<button class="upgrades-tab rebirth-tab" id="rebirthBtn" type="button" title="Rebirth">
  ♻️<span>Rebirth</span>
</button>

<div class="modal-backdrop" id="rebirthBackdrop">
  <div class="modal">
    <div class="modal-header">
      <h2>Rebirth</h2>
      <button class="modal-close" id="rebirthCloseBtn" type="button" aria-label="Close">✕</button>
    </div>
    <div class="modal-body" id="rebirthList"></div>
  </div>
</div>

<button class="tutorial-tab" id="tutorialBtn" type="button" title="How to Play">
  ❓<span>Guide</span>
</button>

<div class="tutorial-panel" id="tutorialPanel">
  <div class="tutorial-panel-header">
    <h2>How to Play</h2>
    <button class="modal-close" id="tutorialCloseBtn" type="button" aria-label="Close">✕</button>
  </div>
  <div class="tutorial-panel-body">
    <section>
      <h3>🌱 Planting</h3>
      <p>Pick a seed from the shelf, then tap any empty plot in your field to plant it.</p>
    </section>
    <section>
      <h3>✨ Mutations</h3>
      <p>Every plant rolls a mutation the moment you plant it — watch for a glowing plot and an icon badge. Multiple tiers can stack together for huge combined value.</p>
    </section>
    <section>
      <h3>☀️ Weather</h3>
      <p>Weather cycles automatically and affects grow speed, sell prices, and mutation odds — check the badge next to your wallet.</p>
    </section>
    <section>
      <h3>🎒 Inventory</h3>
      <p>Harvesting doesn't sell instantly — crops go to your Inventory first. Sell them one at a time or all at once whenever you like.</p>
    </section>
    <section>
      <h3>🛠 Skill Tree</h3>
      <p>Spend coins on permanent-for-this-run upgrades: faster growth, better prices, extra plots, and more. Unlock the root node first.</p>
    </section>
    <section>
      <h3>🧴 Gear Shop</h3>
      <p>Buy consumables like fertilizers or mutation charms, tap one to arm it, then tap a specific growing plot to apply it there.</p>
    </section>
    <section>
      <h3>📜 Quests</h3>
      <p>3 quests are always active. Complete one for XP and coins, and a fresh quest rolls in immediately — they get harder as you level up.</p>
    </section>
    <section>
      <h3>⭐ Leveling</h3>
      <p>Planting, harvesting, and buying upgrades all earn XP. Higher levels unlock rarer, more valuable crops.</p>
    </section>
    <section>
      <h3>♻️ Rebirth</h3>
      <p>Once you reach max level, you can rebirth: it resets your whole run, but pays out permanent rebirth points — 1 per million coins you're holding — to spend on a permanent upgrade shop.</p>
    </section>
  </div>
</div>

<button class="tutorial-tab settings-tab" id="settingsBtn" type="button" title="Settings">
  ⚙️<span>Settings</span>
</button>

<div class="tutorial-panel" id="settingsPanel">
  <div class="tutorial-panel-header">
    <h2>Settings</h2>
    <button class="modal-close" id="settingsCloseBtn" type="button" aria-label="Close">✕</button>
  </div>
  <div class="tutorial-panel-body" id="settingsBody"></div>
</div>

<button class="tabs-toggle-btn" id="tabsToggleBtn" type="button" title="Hide/show side panels">🙈</button>

<div class="toast" id="toast"></div>

<script>
  // unlockLevel = player level required before this seed appears in the shelf
  // regrows   = how many extra times a plot auto-replants itself after harvest (bushes/vines), 0 = one-and-done
  const CROPS = {
    carrot:     { name: 'Carrot',     emoji: '🥕', seedCost: 15,   growMs: 8000,   sellPrice: 22,  unlockLevel: 1,    regrows: 0 },
    potato:     { name: 'Potato',     emoji: '🥔', seedCost: 24,   growMs: 12000,  sellPrice: 36,  unlockLevel: 2,   regrows: 0 },
    strawberry: { name: 'Strawberry', emoji: '🍓', seedCost: 36,  growMs: 16000,  sellPrice: 54,  unlockLevel: 3,   regrows: 3 },
    tomato:     { name: 'Tomato',     emoji: '🍅', seedCost: 45,  growMs: 20000,  sellPrice: 68,  unlockLevel: 4,  regrows: 2 },
    corn:       { name: 'Corn',       emoji: '🌽', seedCost: 60,  growMs: 25000,  sellPrice: 90,  unlockLevel: 5,  regrows: 0 },
    eggplant:   { name: 'Eggplant',   emoji: '🍆', seedCost: 75,  growMs: 30000,  sellPrice: 112,  unlockLevel: 6,  regrows: 1 },
    pepper:     { name: 'Pepper',     emoji: '🌶️', seedCost: 90,  growMs: 35000,  sellPrice: 135,  unlockLevel: 7,  regrows: 2 },
    pineapple:  { name: 'Pineapple',  emoji: '🍍', seedCost: 105,  growMs: 40000,  sellPrice: 158,  unlockLevel: 8,  regrows: 0 },
    pumpkin:    { name: 'Pumpkin',    emoji: '🎃', seedCost: 120,  growMs: 45000,  sellPrice: 180, unlockLevel: 9, regrows: 0 },
    watermelon: { name: 'Watermelon', emoji: '🍉', seedCost: 180,  growMs: 60000,  sellPrice: 270, unlockLevel: 10, regrows: 0 },
    grape:      { name: 'Grape',      emoji: '🍇', seedCost: 240,  growMs: 75000,  sellPrice: 360, unlockLevel: 11, regrows: 4 },
    coconut:    { name: 'Coconut',    emoji: '🥥', seedCost: 300, growMs: 90000,  sellPrice: 450, unlockLevel: 12, regrows: 0 },
    mango:      { name: 'Mango',      emoji: '🥭', seedCost: 390, growMs: 100000, sellPrice: 585, unlockLevel: 13, regrows: 2 },
    cherry:     { name: 'Cherry',     emoji: '🍒', seedCost: 450, growMs: 110000, sellPrice: 675, unlockLevel: 14, regrows: 3 },
    peach:      { name: 'Peach',      emoji: '🍑', seedCost: 540, growMs: 120000, sellPrice: 810, unlockLevel: 15, regrows: 1 },
    kiwi:       { name: 'Kiwi',       emoji: '🥝', seedCost: 630, growMs: 130000, sellPrice: 945, unlockLevel: 16, regrows: 2 },
    avocado:    { name: 'Avocado',    emoji: '🥑', seedCost: 750, growMs: 140000, sellPrice: 1125, unlockLevel: 17, regrows: 0 },
    mushroom:   { name: 'Mushroom',   emoji: '🍄', seedCost: 900,  growMs: 150000, sellPrice: 1350,  unlockLevel: 18, regrows: 4 },
    dragonfruit:{ name: 'Dragonfruit',emoji: '🐉', seedCost: 1100, growMs: 160000, sellPrice: 1650,  unlockLevel: 19, regrows: 0 },
    papaya:     { name: 'Papaya',     emoji: '🍈', seedCost: 1300, growMs: 170000, sellPrice: 1950,  unlockLevel: 20, regrows: 2 },
    starfruit:  { name: 'Starfruit',  emoji: '⭐', seedCost: 1550, growMs: 180000, sellPrice: 2325,  unlockLevel: 21, regrows: 0 },
    truffle:    { name: 'Truffle',    emoji: '🟤', seedCost: 1850, growMs: 190000, sellPrice: 2775, unlockLevel: 22, regrows: 0 },
    saffron:    { name: 'Saffron',    emoji: '🌸', seedCost: 2200, growMs: 200000, sellPrice: 3300, unlockLevel: 23, regrows: 3 },
    durian:     { name: 'Durian',     emoji: '💚', seedCost: 2600, growMs: 210000, sellPrice: 3900, unlockLevel: 24, regrows: 0 },
    // Rebirth-exclusive crops — gated by how many times you've rebirthed, not by level.
    phoenixFruit: { name: 'Phoenix Fruit', emoji: '🔥', seedCost: 5000,   growMs: 240000, sellPrice: 12000,  unlockLevel: 1, rebirthRequired: 1,  regrows: 5 },
    lottoCard:    { name: 'Lotto Card',    emoji: '🎫', seedCost: 8000,   growMs: 255000, sellPrice: 19000,  unlockLevel: 1, rebirthRequired: 2,  regrows: 0 },
    starSeed:     { name: 'Star Seed',     emoji: '🌟', seedCost: 12000,  growMs: 270000, sellPrice: 28000,  unlockLevel: 1, rebirthRequired: 3,  regrows: 0 },
    cakePlant:    { name: 'Cake Plant',    emoji: '🎂', seedCost: 19000,  growMs: 285000, sellPrice: 45000,  unlockLevel: 1, rebirthRequired: 4,  regrows: 2 },
    eternalRoot:  { name: 'Eternal Root',  emoji: '🌳', seedCost: 30000,  growMs: 300000, sellPrice: 70000,  unlockLevel: 1, rebirthRequired: 5,  regrows: 0 },
    goldenGoose:  { name: 'Golden Goose',  emoji: '🦢', seedCost: 50000,  growMs: 315000, sellPrice: 120000, unlockLevel: 1, rebirthRequired: 7,  regrows: 4 },
    voidBlossom:  { name: 'Void Blossom',  emoji: '🖤', seedCost: 80000,  growMs: 330000, sellPrice: 190000, unlockLevel: 1, rebirthRequired: 10, regrows: 3 },
    trophyPlant:  { name: 'Trophy Plant',  emoji: '🏆', seedCost: 150000, growMs: 345000, sellPrice: 360000, unlockLevel: 1, rebirthRequired: 15, regrows: 0 },
    diamondRing:  { name: 'Diamond Ring',  emoji: '💍', seedCost: 280000, growMs: 360000, sellPrice: 670000, unlockLevel: 1, rebirthRequired: 20, regrows: 0 },
  };

  // Mutations roll on every harvest — a lucky variant multiplies that unit's sell value.
  // Checked rarest-first as independent rolls, so only one mutation applies per harvest.
  const MUTATIONS = {
    normal:     { label: 'Normal',     icon: '',   multiplier: 1,    baseChance: 0 },
    giant:      { label: 'Giant',      icon: '📏', multiplier: 1.5,  baseChance: 0.12 },
    golden:     { label: 'Golden',     icon: '✨', multiplier: 2,    baseChance: 0.08 },
    rainbow:    { label: 'Rainbow',    icon: '🌈', multiplier: 4,    baseChance: 0.02 },
    crystal:    { label: 'Crystal',    icon: '💎', multiplier: 8,    baseChance: 0.006 },
    diamond:    { label: 'Diamond',    icon: '🔷', multiplier: 15,   baseChance: 0.002 },
    cosmic:     { label: 'Cosmic',     icon: '🌌', multiplier: 30,   baseChance: 0.0006 },
    celestial:  { label: 'Celestial',  icon: '👑', multiplier: 60,   baseChance: 0.00015 },
    voidtouched:{ label: 'Voidtouched',icon: '🕳️', multiplier: 120,  baseChance: 0.00003 },
  };

  // Weather cycles automatically and affects grow speed, sell prices, and mutation odds.
  const WEATHER_DURATION_MS = 90 * 1000;
  const WEATHER = {
    sunny:   { label: 'Sunny',   icon: '☀️', growthMult: 1.10, sellMult: 1.00, mutationBoost: {},               weight: 40 },
    rainy:   { label: 'Rainy',   icon: '🌧️', growthMult: 1.15, sellMult: 1.00, mutationBoost: { giant: 0.10 },   weight: 25 },
    storm:   { label: 'Storm',   icon: '⛈️', growthMult: 0.85, sellMult: 1.00, mutationBoost: { golden: 0.10 },  weight: 15 },
    frost:   { label: 'Frost',   icon: '❄️', growthMult: 0.75, sellMult: 1.00, mutationBoost: {},               weight: 15 },
    rainbow: { label: 'Rainbow', icon: '🌈', growthMult: 1.20, sellMult: 1.15, mutationBoost: { rainbow: 0.15, crystal: 0.01, diamond: 0.003 }, weight: 5 },
  };

  function pickWeatherKey() {
    const entries = Object.entries(WEATHER);
    const totalWeight = entries.reduce((sum, [, w]) => sum + w.weight, 0);
    let roll = Math.random() * totalWeight;
    for (const [key, w] of entries) {
      roll -= w.weight;
      if (roll <= 0) return key;
    }
    return entries[0][0];
  }

  // Checked rarest-first so a lucky roll can't get "downgraded" by a more common check firing first.
  const MUTATION_ROLL_ORDER = ['voidtouched', 'celestial', 'cosmic', 'diamond', 'crystal', 'rainbow', 'golden', 'giant'];

  // Rolls every mutation tier independently, so a harvest can stack several
  // at once (e.g. Giant AND Golden together) — returns an array of hit keys,
  // empty if none hit (a plain "normal" crop).
  function rollMutations() {
    const boost = WEATHER[state.weather].mutationBoost;
    const rebirthMutationBonus = rebirthBonus('mutationBoost');
    const hits = [];
    for (const key of Object.keys(MUTATIONS)) {
      if (key === 'normal') continue;
      const chance = MUTATIONS[key].baseChance + (boost[key] || 0) + rebirthMutationBonus;
      if (Math.random() < chance) hits.push(key);
    }
    return hits;
  }

  // A "combo key" is how a stack of mutations is stored/displayed: the hit
  // keys joined with "+" (declaration order, for stability), or 'normal' for none.
  function comboKey(hits) {
    return hits.length ? hits.join('+') : 'normal';
  }

  function comboMultiplier(combo) {
    if (combo === 'normal') return 1;
    return combo.split('+').reduce((m, k) => m * (MUTATIONS[k] ? MUTATIONS[k].multiplier : 1), 1);
  }

  function comboLabel(combo) {
    if (combo === 'normal') return '';
    return combo.split('+').map(k => `${MUTATIONS[k].icon} ${MUTATIONS[k].label}`).join(' ');
  }

  function comboIcon(combo) {
    if (combo === 'normal') return null;
    // Lead with the rarest tier present, rarest-first per MUTATION_ROLL_ORDER.
    const parts = combo.split('+');
    for (const key of MUTATION_ROLL_ORDER) {
      if (parts.includes(key)) return MUTATIONS[key].icon;
    }
    return MUTATIONS[parts[0]].icon;
  }

  // Every icon in a stacked combo, rarest-first, so a Giant+Golden+Rainbow plant
  // shows all three emoji rather than just the rarest one.
  function comboIcons(combo) {
    if (combo === 'normal') return '';
    const parts = combo.split('+');
    const ordered = MUTATION_ROLL_ORDER.filter(key => parts.includes(key));
    return ordered.map(key => MUTATIONS[key].icon).join('');
  }

  function comboCssClass(combo) {
    if (combo === 'normal') return '';
    const parts = combo.split('+');
    for (const key of MUTATION_ROLL_ORDER) {
      if (parts.includes(key)) return 'mutation-' + key;
    }
    return 'mutation-' + parts[0];
  }

  // --- XP / Leveling ---
  function xpForLevel(level) {
    return Math.round(80 * Math.pow(1.25, level - 1));
  }

  function addXp(rawAmount) {
    const amount = Math.round(rawAmount * (1 + rebirthBonus('xpBoost')));
    const previouslyUnlocked = new Set(Object.keys(CROPS).filter(isUnlocked));
    state.xp += amount;
    let leveledUp = false;
    while (state.xp >= xpForLevel(state.level)) {
      state.xp -= xpForLevel(state.level);
      state.level += 1;
      const bonus = state.level * 20;
      state.coins += bonus;
      leveledUp = true;
      playSound('levelup');
      setTimeout(() => showToast(`🎉 Level up! You're now level ${state.level} (+${bonus} 🪙)`), 200);
    }
    if (leveledUp) {
      const newlyUnlocked = Object.keys(CROPS).filter(k => isUnlocked(k) && !previouslyUnlocked.has(k));
      if (newlyUnlocked.length > 0) {
        const names = newlyUnlocked.map(k => `${CROPS[k].emoji} ${CROPS[k].name}`).join(', ');
        setTimeout(() => showToast(`New seed unlocked: ${names}!`), 900);
      }
    }
    return leveledUp;
  }

  // --- Quest board ---
  // Each template describes a stat to track progress against; "statKey" reads either a
  // top-level state field (like totalEarned) or one of state.stats.*. Quests measure
  // progress from a baseline snapshot taken when the quest was generated, so slots can be
  // refreshed independently.
  const QUEST_TEMPLATES = [
    { key: 'harvest',   icon: '🌾', label: (n) => `Harvest ${n} crops`,           statKey: 'totalHarvested',       baseTarget: 5,  targetGrowth: 2,  rewardXp: 30, rewardCoins: 40 },
    { key: 'plant',     icon: '🌱', label: (n) => `Plant ${n} seeds`,             statKey: 'totalPlanted',         baseTarget: 5,  targetGrowth: 2,  rewardXp: 25, rewardCoins: 30 },
    { key: 'sell',      icon: '💰', label: (n) => `Earn ${n} 🪙 from selling`,    statKey: 'totalEarned',          baseTarget: 100, targetGrowth: 60, rewardXp: 45, rewardCoins: 20 },
    { key: 'mutation',  icon: '✨', label: (n) => `Find ${n} mutated crop${n > 1 ? 's' : ''}`, statKey: 'totalMutatedHarvests', baseTarget: 2,  targetGrowth: 1,  rewardXp: 55, rewardCoins: 60 },
    { key: 'upgrade',   icon: '🛠️', label: (n) => `Buy ${n} upgrade${n > 1 ? 's' : ''}`,        statKey: 'upgradesBought',       baseTarget: 1,  targetGrowth: 1,  rewardXp: 40, rewardCoins: 25 },
  ];

  function getStatValue(statKey) {
    return statKey === 'totalEarned' ? state.totalEarned : (state.stats[statKey] || 0);
  }

  function questTemplate(quest) {
    return QUEST_TEMPLATES.find(t => t.key === quest.templateKey);
  }

  function questProgress(quest) {
    const t = questTemplate(quest);
    return Math.max(0, Math.min(quest.target, getStatValue(t.statKey) - quest.baseline));
  }

  function makeQuest(template) {
    // Targets scale exponentially with level (not just linearly), so quests get
    // meaningfully harder — not just slightly bigger — the further you progress.
    // Rewards scale up alongside them so high-level quests stay worth doing, and
    // both are locked in at generation time so a quest doesn't shift under you.
    const levelFactor = Math.pow(1.08, state.level - 1);
    const target = Math.max(1, Math.round((template.baseTarget + template.targetGrowth * (state.level - 1)) * levelFactor));
    const rewardMult = 1 + (state.level - 1) * 0.15;
    return {
      id: `${template.key}-${Date.now()}-${Math.random().toString(36).slice(2, 7)}`,
      templateKey: template.key,
      baseline: getStatValue(template.statKey),
      target,
      rewardXp: Math.round(template.rewardXp * rewardMult),
      rewardCoins: Math.round(template.rewardCoins * rewardMult),
      claimed: false,
    };
  }

  function fillQuestSlots() {
    while (state.quests.length < 3) {
      const usedKeys = new Set(state.quests.map(q => q.templateKey));
      const options = QUEST_TEMPLATES.filter(t => !usedKeys.has(t.key));
      const pool = options.length > 0 ? options : QUEST_TEMPLATES;
      const template = pool[Math.floor(Math.random() * pool.length)];
      state.quests.push(makeQuest(template));
    }
  }

  function claimQuest(questId) {
    const quest = state.quests.find(q => q.id === questId);
    if (!quest) return;
    if (questProgress(quest) < quest.target) return;

    const t = questTemplate(quest);
    state.coins += quest.rewardCoins;
    state.quests = state.quests.filter(q => q.id !== questId);
    fillQuestSlots();
    addXp(quest.rewardXp);
    showToast(`Quest complete: ${t.label(quest.target)} — +${quest.rewardXp} XP, +${quest.rewardCoins} 🪙`);
    renderAll();
    if (typeof questsBackdrop !== 'undefined' && questsBackdrop.classList.contains('open')) renderQuests();
  }

  // --- Rebirth ---
  // Resets almost everything (level, coins, seeds, inventory, plots, the skill tree) but
  // pays out permanent "rebirth points" spent on a small, powerful, permanent upgrade shop
  // that survives every future rebirth.
  // Must reach the level of the last crop unlock (the game's current "max level") to rebirth.
  // --- Gear shop ---
  // Consumable items bought with coins, then applied to one specific growing plot —
  // either to speed it up, or to guarantee it comes out with at least a given mutation tier.
  const GEAR_ITEMS = {
    quickFertilizer: {
      name: 'Quick Fertilizer', icon: '💧',
      desc: "Cuts a plot's remaining grow time by 25%",
      cost: 20, effect: { type: 'speed', amount: 0.25 },
    },
    superFertilizer: {
      name: 'Super Fertilizer', icon: '🧪',
      desc: "Cuts a plot's remaining grow time by 50%",
      cost: 60, effect: { type: 'speed', amount: 0.5 },
    },
    instantGrowth: {
      name: 'Instant Growth Potion', icon: '⏱️',
      desc: 'Instantly finishes growing a plot',
      cost: 150, effect: { type: 'instant' },
    },
    goldenCharm: {
      name: 'Golden Charm', icon: '✨',
      desc: "Guarantees a plot's crop comes out at least Golden",
      cost: 100, effect: { type: 'mutation', tier: 'golden' },
    },
    rainbowCharm: {
      name: 'Rainbow Charm', icon: '🌈',
      desc: "Guarantees a plot's crop comes out at least Rainbow",
      cost: 300, effect: { type: 'mutation', tier: 'rainbow' },
    },
    crystalCharm: {
      name: 'Crystal Charm', icon: '💎',
      desc: "Guarantees a plot's crop comes out at least Crystal",
      cost: 800, effect: { type: 'mutation', tier: 'crystal' },
    },
  };

  function buyGear(key) {
    const item = GEAR_ITEMS[key];
    if (state.coins < item.cost) {
      playSound('error');
      showToast(`Not enough coins for ${item.name}`);
      return;
    }
    state.coins -= item.cost;
    state.gear[key] = (state.gear[key] || 0) + 1;
    playSound('buy');
    showToast(`Bought ${item.icon} ${item.name}`);
    renderAll();
    if (typeof gearBackdrop !== 'undefined' && gearBackdrop.classList.contains('open')) renderGearShop();
  }

  function selectGear(key) {
    if ((state.gear[key] || 0) < 1) return;
    state.selectedGearItem = state.selectedGearItem === key ? null : key;
    renderGearShop();
  }

  function applyGearToPlot(index) {
    const key = state.selectedGearItem;
    if (!key) return;
    const plot = state.plots[index];
    if (!plot.crop) {
      showToast('Select a growing plot to use gear on');
      return;
    }
    if ((state.gear[key] || 0) < 1) {
      state.selectedGearItem = null;
      return;
    }

    const item = GEAR_ITEMS[key];
    if (item.effect.type === 'speed') {
      const growMs = effectiveGrowMs(plot.crop);
      const elapsed = Date.now() - plot.plantedAt;
      const remaining = Math.max(0, growMs - elapsed);
      plot.plantedAt -= Math.round(remaining * item.effect.amount);
      showToast(`Used ${item.icon} ${item.name} — sped up growth!`);
    } else if (item.effect.type === 'instant') {
      plot.plantedAt = Date.now() - effectiveGrowMs(plot.crop);
      showToast(`Used ${item.icon} ${item.name} — fully grown!`);
    } else if (item.effect.type === 'mutation') {
      const tier = item.effect.tier;
      const current = (!plot.mutationCombo || plot.mutationCombo === 'normal') ? [] : plot.mutationCombo.split('+');
      if (!current.includes(tier)) current.push(tier);
      plot.mutationCombo = comboKey(current);
      showToast(`Used ${item.icon} ${item.name} — guaranteed at least ${MUTATIONS[tier].label}!`);
    }

    state.gear[key] -= 1;
    if (state.gear[key] <= 0) state.selectedGearItem = null;
    renderAll();
    if (typeof gearBackdrop !== 'undefined' && gearBackdrop.classList.contains('open')) renderGearShop();
  }

  const MIN_REBIRTH_LEVEL = Math.max(...Object.values(CROPS).map(c => c.unlockLevel));

  const REBIRTH_UPGRADES = {
    headStart: {
      name: 'Head Start', icon: '🎒',
      desc: 'Start every rebirth with 2 more free carrot seeds and 25 bonus coins',
      baseCost: 1, costMult: 1.5, maxLevel: 10,
      effectPerLevel: { startSeeds: 2, startCoins: 25 },
    },
    timeWarp: {
      name: 'Time Warp', icon: '⏳',
      desc: 'Permanent +3% grow speed per level — stacks across every rebirth',
      baseCost: 2, costMult: 1.6, maxLevel: 10,
      effectPerLevel: { growthSpeed: 0.03 },
    },
    coinMagnet: {
      name: 'Coin Magnet', icon: '🧲',
      desc: 'Permanent +3% sell prices per level — stacks across every rebirth',
      baseCost: 2, costMult: 1.6, maxLevel: 10,
      effectPerLevel: { sellBoost: 0.03 },
    },
    wisdomKeeper: {
      name: 'Wisdom Keeper', icon: '📖',
      desc: 'Permanent +5% XP gained per level — stacks across every rebirth',
      baseCost: 2, costMult: 1.6, maxLevel: 10,
      effectPerLevel: { xpBoost: 0.05 },
    },
    fortuneFavor: {
      name: "Fortune's Favor", icon: '🍀',
      desc: 'Permanent +0.3% chance for every mutation tier per level',
      baseCost: 3, costMult: 1.7, maxLevel: 8,
      effectPerLevel: { mutationBoost: 0.003 },
    },
  };

  function rebirthBonus(statName) {
    return Object.entries(REBIRTH_UPGRADES).reduce((sum, [key, u]) => {
      const level = state.rebirthUpgrades[key] || 0;
      return sum + level * (u.effectPerLevel[statName] || 0);
    }, 0);
  }

  function rebirthUpgradeCost(key) {
    const u = REBIRTH_UPGRADES[key];
    const level = state.rebirthUpgrades[key] || 0;
    return Math.ceil(u.baseCost * Math.pow(u.costMult, level));
  }

  function calculateRebirthPoints() {
    // 1 rebirth point per million coins currently held — rebirth resets your coins anyway,
    // so this rewards actually banking up a fortune before you pull the trigger.
    return Math.floor(state.coins / 1_000_000);
  }

  function resetRunState() {
    const bonusSeeds = rebirthBonus('startSeeds');
    const bonusCoins = rebirthBonus('startCoins');
    state.coins = bonusCoins;
    state.totalEarned = 0;
    state.seeds = Object.fromEntries(Object.keys(CROPS).map(k => [k, k === 'carrot' ? 3 + bonusSeeds : 0]));
    state.inventory = Object.fromEntries(Object.keys(CROPS).map(k => [k, Object.fromEntries(Object.keys(MUTATIONS).map(m => [m, 0]))]));
    state.plots = Array.from({ length: NUM_PLOTS }, () => ({ crop: null, plantedAt: null, regrowsLeft: 0 }));
    state.selectedSeed = 'carrot';
    state.upgrades = Object.fromEntries(Object.keys(UPGRADES).map(k => [k, UPGRADES[k].repeatable ? 0 : false]));
    state.selectedUpgradeNode = null;
    state.weather = pickWeatherKey();
    state.weatherUntil = Date.now() + WEATHER_DURATION_MS;
    state.xp = 0;
    state.level = 1;
    state.stats = { totalHarvested: 0, totalPlanted: 0, totalMutatedHarvests: 0, upgradesBought: 0 };
    state.quests = [];
    state.gear = Object.fromEntries(Object.keys(GEAR_ITEMS).map(k => [k, 0]));
    state.selectedGearItem = null;
    fillQuestSlots();
  }

  // Populated right when a rebirth breaks the chains on new rebirth-exclusive crops;
  // renderShelf consumes this once (to play the break animation) then clears it.
  let justUnlockedRebirthCrops = [];

  function performRebirth() {
    if (state.level < MIN_REBIRTH_LEVEL) {
      showToast(`Reach max level (${MIN_REBIRTH_LEVEL}) before you can rebirth`);
      return;
    }
    const pointsEarned = calculateRebirthPoints();
    const rebirthsBefore = state.rebirths;
    resetRunState();
    state.rebirths += 1;
    state.rebirthPoints += pointsEarned;

    justUnlockedRebirthCrops = Object.keys(CROPS).filter(k => {
      const req = CROPS[k].rebirthRequired || 0;
      return req > rebirthsBefore && req <= state.rebirths;
    });

    playSound('rebirth');
    showToast(`🌟 Rebirth complete! Earned ${pointsEarned} rebirth point${pointsEarned === 1 ? '' : 's'}.`);
    if (justUnlockedRebirthCrops.length > 0) {
      const names = justUnlockedRebirthCrops.map(k => `${CROPS[k].emoji} ${CROPS[k].name}`).join(', ');
      setTimeout(() => { playSound('chainbreak'); showToast(`⛓️💥 Chains broken! Unlocked: ${names}`); }, 900);
      // Let the break animation play once, then clear the flag so cards settle back to normal.
      setTimeout(() => {
        justUnlockedRebirthCrops = [];
        renderShelf();
      }, 1500);
    }
    renderAll();
  }

  function buyRebirthUpgrade(key) {
    const u = REBIRTH_UPGRADES[key];
    const level = state.rebirthUpgrades[key] || 0;
    if (level >= u.maxLevel) return;
    const cost = rebirthUpgradeCost(key);
    if (state.rebirthPoints < cost) {
      playSound('error');
      showToast(`Not enough rebirth points for ${u.name}`);
      return;
    }
    state.rebirthPoints -= cost;
    state.rebirthUpgrades[key] = level + 1;
    playSound('buy');
    showToast(`Upgraded ${u.icon} ${u.name} to level ${state.rebirthUpgrades[key]}`);
    renderAll();
    renderRebirth();
  }

  const NUM_PLOTS = 9;

  // Upgrade tree: each node (except extraPlot, which repeats) is bought once and requires its parent owned first.
  const UPGRADES = {
    roots: {
      name: 'Tilled Soil',
      icon: '🌱',
      desc: 'Unlocks the upgrade tree',
      cost: 50,
      parent: null,
      repeatable: false,
      effect: {},
    },
    extraPlot: {
      name: 'Extra Plot',
      icon: '➕',
      desc: 'Till one more patch of land to farm on',
      baseCost: 120,
      costMult: 1.55,
      maxLevel: 8,
      parent: 'roots',
      repeatable: true,
    },
    fertilizerI: {
      name: 'Fertilizer I',
      icon: '⚡',
      desc: 'Crops grow 15% faster',
      cost: 220,
      parent: 'roots',
      repeatable: false,
      effect: { growthSpeed: 0.15 },
    },
    fertilizerII: {
      name: 'Fertilizer II',
      icon: '⚡⚡',
      desc: 'Crops grow another 15% faster',
      cost: 650,
      parent: 'fertilizerI',
      repeatable: false,
      effect: { growthSpeed: 0.15 },
    },
    greenhouse: {
      name: 'Greenhouse',
      icon: '🏡',
      desc: 'Crops grow another 20% faster — the big payoff',
      cost: 1600,
      parent: 'fertilizerII',
      repeatable: false,
      effect: { growthSpeed: 0.20 },
    },
    marketI: {
      name: 'Market Contacts I',
      icon: '💰',
      desc: 'Sell prices +15%',
      cost: 280,
      parent: 'roots',
      repeatable: false,
      effect: { sellBoost: 0.15 },
    },
    marketII: {
      name: 'Market Contacts II',
      icon: '💰💰',
      desc: 'Sell prices +15% more',
      cost: 850,
      parent: 'marketI',
      repeatable: false,
      effect: { sellBoost: 0.15 },
    },
    exportDeals: {
      name: 'Export Deals',
      icon: '🚢',
      desc: 'Sell prices +25% more — the big payoff',
      cost: 2000,
      parent: 'marketII',
      repeatable: false,
      effect: { sellBoost: 0.25 },
    },
    solarPanels: {
      name: 'Solar Panels',
      icon: '☀️',
      desc: 'Crops grow another 20% faster — the ultimate speed boost',
      cost: 4000,
      parent: 'greenhouse',
      repeatable: false,
      effect: { growthSpeed: 0.20 },
    },
    globalTrade: {
      name: 'Global Trade',
      icon: '🌍',
      desc: 'Sell prices +30% more — the ultimate profit boost',
      cost: 4500,
      parent: 'exportDeals',
      repeatable: false,
      effect: { sellBoost: 0.30 },
    },
    luckyCharm: {
      name: 'Lucky Charm',
      icon: '🍀',
      desc: 'Each level adds a chance for a harvest to yield a bonus crop',
      baseCost: 200,
      costMult: 1.6,
      maxLevel: 6,
      parent: 'roots',
      repeatable: true,
    },
    greenThumb: {
      name: 'Green Thumb',
      icon: '🌿',
      desc: 'Regrowing crops get +1 extra regrow cycle',
      cost: 300,
      parent: 'roots',
      repeatable: false,
      effect: { regrowBonus: 1 },
    },
    masterFarmer: {
      name: 'Master Farmer',
      icon: '👩‍🌾',
      desc: 'Regrowing crops get +1 more regrow cycle',
      cost: 900,
      parent: 'greenThumb',
      repeatable: false,
      effect: { regrowBonus: 1 },
    },
    seedBank: {
      name: 'Seed Bank',
      icon: '🏦',
      desc: 'All seed prices −15%',
      cost: 350,
      parent: 'roots',
      repeatable: false,
      effect: { seedDiscount: 0.15 },
    },
    wholesaleDeals: {
      name: 'Wholesale Deals',
      icon: '📦',
      desc: 'All seed prices −15% more',
      cost: 1000,
      parent: 'seedBank',
      repeatable: false,
      effect: { seedDiscount: 0.15 },
    },
    fertileGrounds: {
      name: 'Fertile Grounds',
      icon: '🟩',
      desc: 'Instantly till 3 extra plots, on top of Extra Plot',
      cost: 500,
      parent: 'extraPlot',
      repeatable: false,
      effect: {},
    },
  };

  // --- Themes, fonts, and sound ---
  const THEMES = {
    default: null, // no overrides — use each file's own built-in :root palette
    dark: {
      '--sky-top': '#1b1f1a', '--sky-bottom': '#12140f',
      '--soil': '#2b1c12', '--soil-dark': '#1a110b',
      '--leaf': '#4f9d5a', '--leaf-dark': '#397743',
      '--sun': '#ffc857', '--card': '#20241d',
      '--ink': '#e8ede6', '--ink-soft': '#9aa89a', '--border': '#333c2f',
    },
    beer: {
      '--sky-top': '#f5c451', '--sky-bottom': '#d99a2b',
      '--soil': '#6b4423', '--soil-dark': '#4a2d16',
      '--leaf': '#c9822a', '--leaf-dark': '#a5661c',
      '--sun': '#ffd54f', '--card': '#fff8e7',
      '--ink': '#3b2712', '--ink-soft': '#8a6a3a', '--border': '#e8cfa0',
    },
  };
  const THEME_VARS = ['--sky-top', '--sky-bottom', '--soil', '--soil-dark', '--leaf', '--leaf-dark', '--sun', '--card', '--ink', '--ink-soft', '--border'];

  const FONTS = {
    default: null, // no overrides — use each file's own built-in font stack
    serif: { heading: "'Merriweather', serif", body: "'Merriweather', serif" },
    mono: { heading: "'Courier New', monospace", body: "'Courier New', monospace" },
    beer: { heading: "'Luckiest Guy', cursive", body: "'Inter', sans-serif" },
  };

  function applyTheme(themeKey) {
    const root = document.documentElement;
    const theme = THEMES[themeKey];
    if (!theme) {
      THEME_VARS.forEach(v => root.style.removeProperty(v));
    } else {
      THEME_VARS.forEach(v => {
        if (theme[v]) root.style.setProperty(v, theme[v]);
      });
    }
    state.settings.theme = themeKey;
  }

  function applyFont(fontKey) {
    const root = document.documentElement;
    const font = FONTS[fontKey];
    if (!font) {
      root.style.removeProperty('--ui-heading-font');
      root.style.removeProperty('--ui-body-font');
    } else {
      root.style.setProperty('--ui-heading-font', font.heading);
      root.style.setProperty('--ui-body-font', font.body);
    }
    state.settings.font = fontKey;
  }

  // Procedural sound effects via Web Audio — no audio files to host or load.
  let audioCtx = null;
  function getAudioCtx() {
    if (!audioCtx) {
      try {
        audioCtx = new (window.AudioContext || window.webkitAudioContext)();
      } catch (err) {
        return null;
      }
    }
    if (audioCtx.state === 'suspended') audioCtx.resume();
    return audioCtx;
  }

  function playTone(freq, duration, waveform, volume) {
    if (!state.settings.soundEnabled) return;
    const ctx = getAudioCtx();
    if (!ctx) return;
    const osc = ctx.createOscillator();
    const gain = ctx.createGain();
    osc.type = waveform || 'sine';
    osc.frequency.value = freq;
    const peak = Math.max(0, Math.min(1, volume * state.settings.soundVolume));
    const now = ctx.currentTime;
    gain.gain.setValueAtTime(peak, now);
    gain.gain.exponentialRampToValueAtTime(0.001, now + duration);
    osc.connect(gain);
    gain.connect(ctx.destination);
    osc.start(now);
    osc.stop(now + duration);
  }

  const SOUND_PRESETS = {
    plant: () => playTone(520, 0.15, 'sine', 0.35),
    harvest: () => playTone(660, 0.18, 'triangle', 0.4),
    mutation: () => { playTone(880, 0.12, 'square', 0.3); setTimeout(() => playTone(1100, 0.15, 'square', 0.3), 90); },
    sell: () => playTone(740, 0.12, 'sine', 0.35),
    buy: () => playTone(320, 0.1, 'sine', 0.3),
    error: () => playTone(150, 0.2, 'sawtooth', 0.25),
    levelup: () => { [520, 660, 880].forEach((f, i) => setTimeout(() => playTone(f, 0.18, 'triangle', 0.4), i * 100)); },
    rebirth: () => { [300, 450, 600, 750, 900].forEach((f, i) => setTimeout(() => playTone(f, 0.2, 'sine', 0.35), i * 80)); },
    chainbreak: () => { playTone(200, 0.08, 'sawtooth', 0.3); setTimeout(() => playTone(700, 0.2, 'triangle', 0.35), 90); },
  };

  function playSound(name) {
    const preset = SOUND_PRESETS[name];
    if (preset) preset();
  }

  const state = {
    coins: 0,
    totalEarned: 0,
    seeds: Object.fromEntries(Object.keys(CROPS).map(k => [k, k === 'carrot' ? 3 : 0])),
    // Each crop's inventory is now a bucket per mutation tier, e.g. { normal: 2, giant: 1, golden: 0, rainbow: 0 }
    inventory: Object.fromEntries(Object.keys(CROPS).map(k => [k, Object.fromEntries(Object.keys(MUTATIONS).map(m => [m, 0]))])),
    plots: Array.from({ length: NUM_PLOTS }, () => ({ crop: null, plantedAt: null, regrowsLeft: 0 })),
    selectedSeed: 'carrot',
    // extraPlot stores a level (repeatable); every other node stores true/false once bought
    upgrades: Object.fromEntries(Object.keys(UPGRADES).map(k => [k, UPGRADES[k].repeatable ? 0 : false])),
    selectedUpgradeNode: null,
    weather: pickWeatherKey(),
    weatherUntil: Date.now() + WEATHER_DURATION_MS,
    xp: 0,
    level: 1,
    stats: { totalHarvested: 0, totalPlanted: 0, totalMutatedHarvests: 0, upgradesBought: 0 },
    quests: [],
    gear: Object.fromEntries(Object.keys(GEAR_ITEMS).map(k => [k, 0])),
    selectedGearItem: null,
    // Rebirth fields — these are the only things a rebirth does NOT reset.
    rebirths: 0,
    rebirthPoints: 0,
    rebirthUpgrades: Object.fromEntries(Object.keys(REBIRTH_UPGRADES).map(k => [k, 0])),
    // Settings — also survive rebirth, since they're about how you play, not game progress.
    settings: { soundEnabled: true, soundVolume: 0.5, theme: 'default', font: 'default' },
  };
  fillQuestSlots();
  applyTheme(state.settings.theme);
  applyFont(state.settings.font);

  function isUnlocked(key) {
    return state.level >= CROPS[key].unlockLevel && state.rebirths >= (CROPS[key].rebirthRequired || 0);
  }

  function isOwned(key) {
    const u = UPGRADES[key];
    return u.repeatable ? state.upgrades[key] > 0 : !!state.upgrades[key];
  }

  function canBuy(key) {
    const u = UPGRADES[key];
    if (u.parent && !isOwned(u.parent)) return false;
    if (!u.repeatable && isOwned(key)) return false;
    if (u.repeatable && state.upgrades[key] >= u.maxLevel) return false;
    return true;
  }

  function nodeCost(key) {
    const u = UPGRADES[key];
    if (!u.repeatable) return u.cost;
    const level = state.upgrades[key] || 0;
    return Math.round(u.baseCost * Math.pow(u.costMult, level));
  }

  function totalGrowthSpeedBoost() {
    return Object.entries(UPGRADES)
      .filter(([key, u]) => !u.repeatable && isOwned(key) && u.effect && u.effect.growthSpeed)
      .reduce((sum, [, u]) => sum + u.effect.growthSpeed, 0);
  }

  function totalSellBoost() {
    return Object.entries(UPGRADES)
      .filter(([key, u]) => !u.repeatable && isOwned(key) && u.effect && u.effect.sellBoost)
      .reduce((sum, [, u]) => sum + u.effect.sellBoost, 0);
  }

  function effectiveGrowMs(cropKey) {
    const reduction = Math.min(0.85, totalGrowthSpeedBoost() + rebirthBonus('growthSpeed'));
    const base = CROPS[cropKey].growMs * (1 - reduction);
    const weatherMult = WEATHER[state.weather].growthMult;
    return Math.max(1000, Math.round(base / weatherMult));
  }

  function effectiveSellPrice(cropKey) {
    const base = CROPS[cropKey].sellPrice * (1 + totalSellBoost() + rebirthBonus('sellBoost'));
    const weatherMult = WEATHER[state.weather].sellMult;
    return Math.round(base * weatherMult);
  }

  function totalRegrowBonus() {
    return Object.entries(UPGRADES)
      .filter(([key, u]) => !u.repeatable && isOwned(key) && u.effect && u.effect.regrowBonus)
      .reduce((sum, [, u]) => sum + u.effect.regrowBonus, 0);
  }

  function totalSeedDiscount() {
    const discount = Object.entries(UPGRADES)
      .filter(([key, u]) => !u.repeatable && isOwned(key) && u.effect && u.effect.seedDiscount)
      .reduce((sum, [, u]) => sum + u.effect.seedDiscount, 0);
    return Math.min(0.6, discount);
  }

  function effectiveSeedCost(cropKey) {
    return Math.max(1, Math.round(CROPS[cropKey].seedCost * (1 - totalSeedDiscount())));
  }

  const walletEl = document.getElementById('wallet');
  const weatherEl = document.getElementById('weatherBadge');
  const shelfEl = document.getElementById('seedShelf');
  const fieldEl = document.getElementById('field');
  const toastEl = document.getElementById('toast');

  let toastTimer = null;
  function showToast(msg) {
    toastEl.textContent = msg;
    toastEl.classList.add('show');
    clearTimeout(toastTimer);
    toastTimer = setTimeout(() => toastEl.classList.remove('show'), 1800);
  }

  function fmtTime(ms) {
    const s = Math.ceil(ms / 1000);
    return s >= 60 ? `${Math.floor(s / 60)}m ${s % 60}s` : `${s}s`;
  }

  function renderShelf() {
    shelfEl.innerHTML = '';
    Object.entries(CROPS).forEach(([key, crop]) => {
      const card = document.createElement('div');
      const unlocked = isUnlocked(key);

      if (!unlocked) {
        const needsRebirth = (crop.rebirthRequired || 0) > state.rebirths;
        const requirementText = needsRebirth
          ? `♻️ Rebirth ${crop.rebirthRequired}x to unlock`
          : `Reach Level ${crop.unlockLevel} to unlock`;
        card.className = 'seed-card locked' + (needsRebirth ? ' rebirth-locked' : '');
        card.innerHTML = `
          <div class="emoji">🔒</div>
          <div class="name">???</div>
          <div class="meta">${requirementText}</div>
        `;
        shelfEl.appendChild(card);
        return;
      }

      const isRebirthExclusive = (crop.rebirthRequired || 0) > 0;
      const justBroke = justUnlockedRebirthCrops.includes(key);
      card.className = 'seed-card' + (state.selectedSeed === key ? ' selected' : '') + (isRebirthExclusive ? ' rebirth-exclusive' : '') + (justBroke ? ' chain-break' : '');
      card.innerHTML = `
        <div class="owned">x${state.seeds[key]}</div>
        ${isRebirthExclusive ? '<div class="rebirth-exclusive-tag">♻️ Rebirth Exclusive</div>' : ''}
        <div class="emoji">${crop.emoji}</div>
        <div class="name">${crop.name}</div>
        <div class="meta">Sells ${effectiveSellPrice(key)} 🪙 · ${fmtTime(effectiveGrowMs(key))}${crop.regrows > 0 ? ` · 🔁x${crop.regrows + totalRegrowBonus()}` : ''}</div>
        <div class="buy-row">
          <button data-buy="${key}" data-amt="1">+1 seed (${effectiveSeedCost(key)}🪙)</button>
          <button data-buy="${key}" data-amt="5">+5 (${effectiveSeedCost(key) * 5}🪙)</button>
        </div>
      `;
      card.addEventListener('click', (e) => {
        if (e.target.closest('button')) return;
        state.selectedSeed = key;
        renderShelf();
      });
      shelfEl.appendChild(card);
    });

    shelfEl.querySelectorAll('button[data-buy]').forEach(btn => {
      const key = btn.getAttribute('data-buy');
      const amt = parseInt(btn.getAttribute('data-amt'), 10);
      const cost = effectiveSeedCost(key) * amt;
      btn.disabled = state.coins < cost;
      btn.addEventListener('click', () => buySeeds(key, amt));
    });
  }

  function buySeeds(key, amt) {
    const cost = effectiveSeedCost(key) * amt;
    if (state.coins < cost) {
      playSound('error');
      showToast(`Not enough coins for ${amt}x ${CROPS[key].name} seeds`);
      return;
    }
    state.coins -= cost;
    state.seeds[key] += amt;
    playSound('buy');
    showToast(`Bought ${amt}x ${CROPS[key].emoji} ${CROPS[key].name} seed${amt > 1 ? 's' : ''}`);
    renderAll();
  }

  function plantPlot(index) {
    const plot = state.plots[index];
    if (plot.crop) return;
    const key = state.selectedSeed;
    if (state.seeds[key] < 1) {
      showToast(`No ${CROPS[key].name} seeds left — buy more!`);
      return;
    }
    state.seeds[key] -= 1;
    plot.crop = key;
    plot.plantedAt = Date.now();
    plot.regrowsLeft = CROPS[key].regrows > 0 ? CROPS[key].regrows + totalRegrowBonus() : 0;
    // Roll the mutation now, at planting, so it can be teased visually while it grows
    // rather than only revealed at harvest.
    plot.mutationCombo = comboKey(rollMutations());
    const mutationHint = plot.mutationCombo !== 'normal' ? ` — looks like it might turn out ${comboLabel(plot.mutationCombo)}!` : '';
    state.stats.totalPlanted += 1;
    addXp(2);
    playSound('plant');
    if (plot.mutationCombo !== 'normal') playSound('mutation');
    showToast(`Planted ${CROPS[key].emoji} ${CROPS[key].name}${mutationHint}`);
    renderAll();
  }

  function sellCrop(key, mutation, amount) {
    const owned = state.inventory[key][mutation] || 0;
    const sellAmount = Math.min(amount, owned);
    if (sellAmount <= 0) return;

    const unitPrice = Math.round(effectiveSellPrice(key) * comboMultiplier(mutation));
    const earned = unitPrice * sellAmount;

    state.coins += earned;
    state.totalEarned += earned;
    state.inventory[key][mutation] -= sellAmount;

    const mutationTag = mutation !== 'normal' ? `${comboLabel(mutation)} ` : '';
    playSound('sell');
    showToast(`Sold ${sellAmount}x ${mutationTag}${CROPS[key].emoji} ${CROPS[key].name} for ${earned} 🪙`);

    renderAll();
    if (inventoryBackdrop.classList.contains('open')) renderInventory();
  }

  function sellAllCrops() {
    const totalOwned = Object.values(state.inventory)
      .reduce((sum, buckets) => sum + Object.values(buckets).reduce((a, b) => a + b, 0), 0);
    if (totalOwned === 0) {
      showToast('Your inventory is empty');
      return;
    }
    Object.keys(state.inventory).forEach(key => {
      Object.keys(state.inventory[key]).forEach(mutation => {
        if (state.inventory[key][mutation] > 0) sellCrop(key, mutation, state.inventory[key][mutation]);
      });
    });
  }

  function harvestPlot(index) {
    const plot = state.plots[index];
    if (!plot.crop) return;
    const crop = CROPS[plot.crop];
    const cropKey = plot.crop;
    const growMs = effectiveGrowMs(plot.crop);
    const elapsed = Date.now() - plot.plantedAt;
    if (elapsed < growMs) return;

    // Use the mutation that was already rolled (and visible) at planting time, rather
    // than rolling a fresh surprise here.
    const combo = plot.mutationCombo || 'normal';
    state.inventory[cropKey][combo] = (state.inventory[cropKey][combo] || 0) + 1;
    const mutationTag = combo !== 'normal' ? ` ${comboLabel(combo)}` : '';

    state.stats.totalHarvested += 1;
    const stackedTiers = combo === 'normal' ? 0 : combo.split('+').length;
    if (stackedTiers > 0) state.stats.totalMutatedHarvests += 1;
    addXp(8 + stackedTiers * 4);
    playSound('harvest');
    if (stackedTiers > 0) playSound('mutation');

    const gotLucky = Math.random() < luckyCharmChance();
    if (gotLucky) {
      const bonusCombo = comboKey(rollMutations());
      state.inventory[cropKey][bonusCombo] = (state.inventory[cropKey][bonusCombo] || 0) + 1;
    }

    if (plot.regrowsLeft > 0) {
      plot.regrowsLeft -= 1;
      plot.plantedAt = Date.now();
      // Each regrowth cycle is a fresh plant, so it gets its own new mutation roll to tease.
      plot.mutationCombo = comboKey(rollMutations());
      showToast(`Harvested${mutationTag} ${crop.emoji} ${crop.name}${gotLucky ? ' — 🍀 lucky bonus crop!' : ''} — it's regrowing! (${plot.regrowsLeft} left). Sell it from your 🎒 Inventory.`);
    } else {
      plot.crop = null;
      plot.plantedAt = null;
      plot.regrowsLeft = 0;
      plot.mutationCombo = null;
      showToast(`Harvested${mutationTag} ${crop.emoji} ${crop.name}${gotLucky ? ' — 🍀 lucky bonus crop!' : ''}! Sell it from your 🎒 Inventory.`);
    }

    renderAll();
  }

  function renderField() {
    const banner = document.getElementById('gearArmedBanner');
    if (state.selectedGearItem) {
      const item = GEAR_ITEMS[state.selectedGearItem];
      banner.style.display = 'flex';
      banner.innerHTML = `
        <span>${item.icon} ${item.name} armed — tap a growing plot to use it</span>
        <button id="gearCancelBtn">Cancel</button>
      `;
      document.getElementById('gearCancelBtn').addEventListener('click', () => {
        state.selectedGearItem = null;
        renderField();
      });
    } else {
      banner.style.display = 'none';
      banner.innerHTML = '';
    }

    fieldEl.innerHTML = '';
    state.plots.forEach((plot, i) => {
      const div = document.createElement('div');
      div.className = 'plot';

      if (!plot.crop) {
        div.innerHTML = `<span class="empty-hint">Tap to plant<br>${CROPS[state.selectedSeed].emoji}</span>`;
        div.addEventListener('click', () => {
          if (state.selectedGearItem) {
            showToast('Select a growing plot to use gear on');
            return;
          }
          plantPlot(i);
        });
      } else {
        const crop = CROPS[plot.crop];
        const growMs = effectiveGrowMs(plot.crop);
        const elapsed = Date.now() - plot.plantedAt;
        const pct = Math.min(100, (elapsed / growMs) * 100);
        const ready = elapsed >= growMs;
        const hasMutation = plot.mutationCombo && plot.mutationCombo !== 'normal';
        if (ready) div.classList.add('ready');
        if (hasMutation) div.classList.add('mutating', comboCssClass(plot.mutationCombo));
        div.innerHTML = `
          ${ready ? '<div class="ready-badge">Ready!</div>' : ''}
          ${plot.regrowsLeft > 0 ? `<div class="regrow-badge">🔁${plot.regrowsLeft}</div>` : ''}
          ${hasMutation ? `<div class="mutation-hint" title="${comboLabel(plot.mutationCombo)}">${comboIcons(plot.mutationCombo)}</div>` : ''}
          <span class="crop-emoji">${crop.emoji}</span>
          <div class="progress-track"><div class="progress-fill" style="width:${pct}%"></div></div>
        `;
        div.addEventListener('click', () => {
          if (state.selectedGearItem) {
            applyGearToPlot(i);
            return;
          }
          harvestPlot(i);
        });
      }
      fieldEl.appendChild(div);
    });
  }

  function renderAll() {
    if (!isUnlocked(state.selectedSeed)) {
      state.selectedSeed = 'carrot';
    }
    walletEl.textContent = `${state.coins} 🪙`;
    renderWeather();
    renderXpBadge();
    renderShelf();
    renderField();
  }

  function renderXpBadge() {
    const xpEl = document.getElementById('xpBadge');
    const fillEl = document.getElementById('xpBadgeFill');
    if (!xpEl || !fillEl) return;
    xpEl.querySelector('.xp-badge-level').textContent = `Lv ${state.level}`;
    const pct = Math.min(100, (state.xp / xpForLevel(state.level)) * 100);
    fillEl.style.width = `${pct}%`;
    xpEl.title = `${state.xp} / ${xpForLevel(state.level)} XP to next level`;
  }

  function renderWeather() {
    const w = WEATHER[state.weather];
    const secsLeft = Math.max(0, Math.ceil((state.weatherUntil - Date.now()) / 1000));
    weatherEl.textContent = `${w.icon} ${w.label} (${secsLeft}s)`;
    weatherEl.title = `Grow speed x${w.growthMult.toFixed(2)}, sell price x${w.sellMult.toFixed(2)}`;
  }

  function checkWeather() {
    if (Date.now() >= state.weatherUntil) {
      state.weather = pickWeatherKey();
      state.weatherUntil = Date.now() + WEATHER_DURATION_MS;
      showToast(`Weather changed: ${WEATHER[state.weather].icon} ${WEATHER[state.weather].label}`);
      renderAll();
    } else {
      renderWeather();
    }
  }

  renderAll();
  setInterval(() => { checkWeather(); renderField(); }, 400); // keep progress bars, ready badges, and weather live

  // --- Inventory ---
  const inventoryBtn = document.getElementById('inventoryBtn');
  const inventoryBackdrop = document.getElementById('inventoryBackdrop');
  const inventoryCloseBtn = document.getElementById('inventoryCloseBtn');
  const inventoryList = document.getElementById('inventoryList');

  function openInventory() {
    renderInventory();
    inventoryBackdrop.classList.add('open');
  }
  function closeInventory() {
    inventoryBackdrop.classList.remove('open');
  }

  inventoryBtn.addEventListener('click', openInventory);
  inventoryCloseBtn.addEventListener('click', closeInventory);
  inventoryBackdrop.addEventListener('click', (e) => {
    if (e.target === inventoryBackdrop) closeInventory();
  });

  function renderInventory() {
    inventoryList.innerHTML = '';

    // Flatten into rows of { key, mutation, count } for every crop+mutation combo you're holding.
    const rows = [];
    Object.entries(state.inventory).forEach(([key, buckets]) => {
      Object.entries(buckets).forEach(([mutation, count]) => {
        if (count > 0) rows.push({ key, mutation, count });
      });
    });

    if (rows.length === 0) {
      const empty = document.createElement('p');
      empty.style.cssText = 'color:var(--ink-soft); font-size:13px; text-align:center; margin:10px 0;';
      empty.textContent = 'Nothing to sell yet — go harvest some crops!';
      inventoryList.appendChild(empty);
      return;
    }

    const sellAllBar = document.createElement('button');
    sellAllBar.textContent = 'Sell everything';
    sellAllBar.style.cssText = 'align-self:flex-start; font-family:Inter,sans-serif; font-size:12px; font-weight:600; padding:8px 14px; border-radius:10px; border:1px solid var(--border); background:var(--leaf); color:#fff; cursor:pointer;';
    sellAllBar.addEventListener('click', sellAllCrops);
    inventoryList.appendChild(sellAllBar);

    rows.forEach(({ key, mutation, count }) => {
      const crop = CROPS[key];
      const mult = comboMultiplier(mutation);
      const unitPrice = Math.round(effectiveSellPrice(key) * mult);
      const label = mutation !== 'normal' ? `${comboLabel(mutation)} ${crop.name}` : crop.name;
      const card = document.createElement('div');
      card.className = 'upgrade-card' + (mutation !== 'normal' ? ' ' + comboCssClass(mutation) : '');
      card.innerHTML = `
        <div class="icon">${mutation !== 'normal' ? comboIcon(mutation) : crop.emoji}</div>
        <div class="info">
          <div class="name">${label} <span style="color:var(--ink-soft); font-weight:500;">x${count}</span></div>
          <div class="desc">${unitPrice} 🪙 each${mutation !== 'normal' ? ` (${mult}x)` : ''}</div>
        </div>
        <div style="display:flex; flex-direction:column; gap:4px;">
          <button data-sell="${key}" data-mutation="${mutation}" data-amt="1">Sell 1</button>
          <button data-sell="${key}" data-mutation="${mutation}" data-amt="${count}">Sell all (${count})</button>
        </div>
      `;
      inventoryList.appendChild(card);
    });

    inventoryList.querySelectorAll('button[data-sell]').forEach(btn => {
      const key = btn.getAttribute('data-sell');
      const mutation = btn.getAttribute('data-mutation');
      const amt = parseInt(btn.getAttribute('data-amt'), 10);
      btn.addEventListener('click', () => sellCrop(key, mutation, amt));
    });
  }

  // --- Quest board ---
  const questsBtn = document.getElementById('questsBtn');
  const questsBackdrop = document.getElementById('questsBackdrop');
  const questsCloseBtn = document.getElementById('questsCloseBtn');
  const questsList = document.getElementById('questsList');

  function openQuests() {
    renderQuests();
    questsBackdrop.classList.add('open');
  }
  function closeQuests() {
    questsBackdrop.classList.remove('open');
  }

  questsBtn.addEventListener('click', openQuests);
  questsCloseBtn.addEventListener('click', closeQuests);
  questsBackdrop.addEventListener('click', (e) => {
    if (e.target === questsBackdrop) closeQuests();
  });

  function renderQuests() {
    questsList.innerHTML = '';
    fillQuestSlots();

    state.quests.forEach(quest => {
      const t = questTemplate(quest);
      const progress = questProgress(quest);
      const done = progress >= quest.target;
      const pct = Math.min(100, (progress / quest.target) * 100);

      const card = document.createElement('div');
      card.className = 'quest-card' + (done ? ' done' : '');
      card.innerHTML = `
        <div class="icon">${t.icon}</div>
        <div class="info">
          <div class="name">${t.label(quest.target)}</div>
          <div class="quest-progress-track"><div class="quest-progress-fill" style="width:${pct}%"></div></div>
          <div class="desc">${progress} / ${quest.target} · reward: ${quest.rewardXp} XP${quest.rewardCoins > 0 ? `, ${quest.rewardCoins} 🪙` : ''}</div>
        </div>
        <button ${done ? '' : 'disabled'} data-claim="${quest.id}">${done ? 'Claim' : 'In progress'}</button>
      `;
      questsList.appendChild(card);
    });

    questsList.querySelectorAll('button[data-claim]').forEach(btn => {
      btn.addEventListener('click', () => claimQuest(btn.getAttribute('data-claim')));
    });
  }

  // --- Gear shop panel ---
  const gearShopBtn = document.getElementById('gearShopBtn');
  const gearBackdrop = document.getElementById('gearBackdrop');
  const gearCloseBtn = document.getElementById('gearCloseBtn');
  const gearShopList = document.getElementById('gearShopList');

  function openGearShop() {
    renderGearShop();
    gearBackdrop.classList.add('open');
  }
  function closeGearShop() {
    gearBackdrop.classList.remove('open');
  }

  gearShopBtn.addEventListener('click', openGearShop);
  gearCloseBtn.addEventListener('click', closeGearShop);
  gearBackdrop.addEventListener('click', (e) => {
    if (e.target === gearBackdrop) closeGearShop();
  });

  function renderGearShop() {
    gearShopList.innerHTML = '';

    const ownedHeading = document.createElement('div');
    ownedHeading.className = 'tree-column-label';
    ownedHeading.style.cssText = 'margin-bottom:8px;';
    ownedHeading.textContent = '🎒 Your Gear (tap to arm, then tap a plot)';
    gearShopList.appendChild(ownedHeading);

    const ownedEntries = Object.entries(state.gear).filter(([, count]) => count > 0);
    if (ownedEntries.length === 0) {
      const none = document.createElement('p');
      none.style.cssText = 'color:var(--ink-soft); font-size:13px; margin:0 0 16px;';
      none.textContent = "You don't have any gear yet — buy some below.";
      gearShopList.appendChild(none);
    } else {
      ownedEntries.forEach(([key, count]) => {
        const item = GEAR_ITEMS[key];
        const armed = state.selectedGearItem === key;
        const card = document.createElement('div');
        card.className = 'upgrade-card' + (armed ? ' owned' : '');
        card.style.cssText = 'cursor:pointer; margin-bottom:8px;';
        card.innerHTML = `
          <div class="icon">${item.icon}</div>
          <div class="info">
            <div class="name">${item.name} <span style="color:var(--ink-soft); font-weight:500;">x${count}</span></div>
            <div class="desc">${armed ? 'Armed — tap a growing plot' : item.desc}</div>
          </div>
        `;
        card.addEventListener('click', () => selectGear(key));
        gearShopList.appendChild(card);
      });
    }

    const shopHeading = document.createElement('div');
    shopHeading.className = 'tree-column-label';
    shopHeading.style.cssText = 'margin:16px 0 8px;';
    shopHeading.textContent = '🧴 Buy Gear';
    gearShopList.appendChild(shopHeading);

    Object.entries(GEAR_ITEMS).forEach(([key, item]) => {
      const card = document.createElement('div');
      card.className = 'upgrade-card';
      card.innerHTML = `
        <div class="icon">${item.icon}</div>
        <div class="info">
          <div class="name">${item.name}</div>
          <div class="desc">${item.desc}</div>
        </div>
        <button ${state.coins < item.cost ? 'disabled' : ''} data-buy-gear="${key}">Buy — ${item.cost} 🪙</button>
      `;
      gearShopList.appendChild(card);
    });

    gearShopList.querySelectorAll('button[data-buy-gear]').forEach(btn => {
      btn.addEventListener('click', () => buyGear(btn.getAttribute('data-buy-gear')));
    });
  }

  // --- Upgrades shop ---
  const upgradesBtn = document.getElementById('upgradesBtn');
  const upgradesBackdrop = document.getElementById('upgradesBackdrop');
  const upgradesCloseBtn = document.getElementById('upgradesCloseBtn');
  const upgradesList = document.getElementById('upgradesList');

  function openUpgrades() {
    renderUpgrades();
    upgradesBackdrop.classList.add('open');
  }
  function closeUpgrades() {
    upgradesBackdrop.classList.remove('open');
  }

  upgradesBtn.addEventListener('click', openUpgrades);
  upgradesCloseBtn.addEventListener('click', closeUpgrades);
  upgradesBackdrop.addEventListener('click', (e) => {
    if (e.target === upgradesBackdrop) closeUpgrades();
  });

  function upgradeEffectLabel(key) {
    const u = UPGRADES[key];
    if (key === 'extraPlot' || key === 'fertileGrounds') return `${state.plots.length} plots owned`;
    if (key === 'luckyCharm') return `${Math.round(luckyCharmChance() * 100)}% bonus-crop chance`;
    if (u.effect && u.effect.growthSpeed) return `−${Math.round(u.effect.growthSpeed * 100)}% grow time`;
    if (u.effect && u.effect.sellBoost) return `+${Math.round(u.effect.sellBoost * 100)}% sell price`;
    if (u.effect && u.effect.regrowBonus) return `+${u.effect.regrowBonus} regrow cycle`;
    if (u.effect && u.effect.seedDiscount) return `−${Math.round(u.effect.seedDiscount * 100)}% seed price`;
    return '';
  }

  function luckyCharmChance() {
    return Math.min(0.3, (state.upgrades.luckyCharm || 0) * 0.05);
  }

  function nodeStateClass(key) {
    if (isOwned(key) && !UPGRADES[key].repeatable) return 'owned';
    if (UPGRADES[key].repeatable && state.upgrades[key] > 0) return 'owned partial';
    if (canBuy(key)) return 'available';
    return 'locked';
  }

  function renderNodeCircle(key) {
    const u = UPGRADES[key];
    const stateClass = nodeStateClass(key);
    const selected = state.selectedUpgradeNode === key ? ' selected' : '';
    const owned = isOwned(key);
    const maxed = u.repeatable && state.upgrades[key] >= u.maxLevel;
    const badge = u.repeatable
      ? `<span class="tree-node-badge">${state.upgrades[key]}/${u.maxLevel}</span>`
      : (owned ? `<span class="tree-node-badge check">✓</span>` : '');

    const btn = document.createElement('button');
    btn.type = 'button';
    btn.className = `tree-node-circle ${stateClass}${selected}`;
    btn.setAttribute('data-node', key);
    btn.innerHTML = `<span class="tree-node-icon">${stateClass === 'locked' ? '🔒' : u.icon}</span>${badge}`;
    btn.addEventListener('click', () => {
      state.selectedUpgradeNode = key;
      // Tapping an affordable, unlocked node buys it immediately; tapping a
      // locked/maxed/already-owned node just opens its details below instead.
      if (canBuy(key) && !maxed && state.coins >= nodeCost(key)) {
        buyUpgrade(key);
      } else {
        renderUpgrades();
      }
    });

    const wrap = document.createElement('div');
    wrap.className = 'tree-node-wrap';
    wrap.appendChild(btn);

    const price = document.createElement('div');
    price.className = 'tree-node-price';
    if (maxed) {
      price.textContent = 'Maxed';
    } else if (owned && !u.repeatable) {
      price.textContent = 'Owned';
    } else {
      price.textContent = `${nodeCost(key)} 🪙`;
    }
    wrap.appendChild(price);

    return wrap;
  }

  function connectorLine() {
    const line = document.createElement('div');
    line.className = 'tree-connector-line';
    return line;
  }

  function renderUpgradeDetail(key) {
    if (!key) {
      return `<p style="color:var(--ink-soft); font-size:13px; text-align:center; margin:0;">Tap a node in the tree to see what it does.</p>`;
    }
    const u = UPGRADES[key];
    const owned = isOwned(key);
    const buyable = canBuy(key);
    const cost = nodeCost(key);
    const locked = !owned && !buyable;
    const maxed = u.repeatable && state.upgrades[key] >= u.maxLevel;

    let buttonHtml;
    if (maxed) {
      buttonHtml = `<button disabled>Maxed</button>`;
    } else if (owned && !u.repeatable) {
      buttonHtml = `<button disabled>Owned</button>`;
    } else if (locked) {
      buttonHtml = `<button disabled>Locked</button>`;
    } else {
      buttonHtml = `<button ${state.coins < cost ? 'disabled' : ''} data-buy="${key}">Buy — ${cost} 🪙</button>`;
    }

    const levelTag = u.repeatable ? ` (Lv ${state.upgrades[key]}/${u.maxLevel})` : (owned ? ' ✓ owned' : '');

    return `
      <div class="upgrade-card${locked ? ' locked' : ''}${owned && !u.repeatable ? ' owned' : ''}">
        <div class="icon">${locked ? '🔒' : u.icon}</div>
        <div class="info">
          <div class="name">${u.name}${levelTag}</div>
          <div class="desc">${locked ? `Requires ${UPGRADES[u.parent].name}` : u.desc}</div>
          ${owned || u.repeatable ? `<div class="level">${upgradeEffectLabel(key)}</div>` : ''}
        </div>
        ${buttonHtml}
      </div>
    `;
  }

  function renderUpgrades() {
    upgradesList.innerHTML = '';

    const tree = document.createElement('div');
    tree.className = 'skill-tree';

    const rootWrap = document.createElement('div');
    rootWrap.className = 'tree-root-wrap';
    rootWrap.appendChild(renderNodeCircle('roots'));
    tree.appendChild(rootWrap);

    tree.appendChild(connectorLine());

    const crossbar = document.createElement('div');
    crossbar.className = 'tree-crossbar';
    tree.appendChild(crossbar);

    const columns = document.createElement('div');
    columns.className = 'tree-columns';

    const branches = [
      { label: '⚡ Growth', chain: ['fertilizerI', 'fertilizerII', 'greenhouse', 'solarPanels'] },
      { label: '➕ Land', chain: ['extraPlot', 'fertileGrounds'] },
      { label: '💰 Profit', chain: ['marketI', 'marketII', 'exportDeals', 'globalTrade'] },
      { label: '🍀 Luck', chain: ['luckyCharm'] },
      { label: '🌾 Harvest', chain: ['greenThumb', 'masterFarmer'] },
      { label: '🏪 Trade', chain: ['seedBank', 'wholesaleDeals'] },
    ];

    branches.forEach(branch => {
      const col = document.createElement('div');
      col.className = 'tree-column';

      const stub = document.createElement('div');
      stub.className = 'tree-stub';
      col.appendChild(stub);

      const label = document.createElement('div');
      label.className = 'tree-column-label';
      label.textContent = branch.label;
      col.appendChild(label);

      branch.chain.forEach((key, i) => {
        if (i > 0) col.appendChild(connectorLine());
        col.appendChild(renderNodeCircle(key));
      });

      columns.appendChild(col);
    });

    tree.appendChild(columns);
    upgradesList.appendChild(tree);

    const detail = document.createElement('div');
    detail.className = 'tree-detail';
    detail.innerHTML = renderUpgradeDetail(state.selectedUpgradeNode);
    upgradesList.appendChild(detail);

    detail.querySelectorAll('button[data-buy]').forEach(btn => {
      btn.addEventListener('click', () => buyUpgrade(btn.getAttribute('data-buy')));
    });
  }

  function buyUpgrade(key) {
    const u = UPGRADES[key];
    if (!canBuy(key)) return;
    const cost = nodeCost(key);
    if (state.coins < cost) {
      playSound('error');
      showToast(`Not enough coins for ${u.name}`);
      return;
    }
    state.coins -= cost;
    playSound('buy');
    state.stats.upgradesBought += 1;
    addXp(15);

    if (u.repeatable) {
      state.upgrades[key] = (state.upgrades[key] || 0) + 1;
      if (key === 'extraPlot') {
        state.plots.push({ crop: null, plantedAt: null, regrowsLeft: 0 });
      }
      showToast(`Upgraded ${u.icon} ${u.name} to level ${state.upgrades[key]}`);
    } else {
      state.upgrades[key] = true;
      if (key === 'fertileGrounds') {
        for (let i = 0; i < 3; i++) {
          state.plots.push({ crop: null, plantedAt: null, regrowsLeft: 0 });
        }
      }
      showToast(`Unlocked ${u.icon} ${u.name}!`);
    }

    renderUpgrades();
    renderAll();
  }



  // --- Show/hide side tabs toggle ---
  const tabsToggleBtn = document.getElementById('tabsToggleBtn');
  tabsToggleBtn.addEventListener('click', () => {
    const hidden = document.body.classList.toggle('tabs-hidden');
    tabsToggleBtn.textContent = hidden ? '👁' : '🙈';
    tabsToggleBtn.title = hidden ? 'Show side panels' : 'Hide side panels';
  });

  // --- Settings panel ---
  const settingsBtn = document.getElementById('settingsBtn');
  const settingsPanel = document.getElementById('settingsPanel');
  const settingsCloseBtn = document.getElementById('settingsCloseBtn');
  const settingsBody = document.getElementById('settingsBody');

  settingsBtn.addEventListener('click', () => {
    renderSettings();
    settingsPanel.classList.toggle('open');
  });
  settingsCloseBtn.addEventListener('click', () => {
    settingsPanel.classList.remove('open');
  });

  function renderSettings() {
    settingsBody.innerHTML = '';

    // Sound
    const soundSection = document.createElement('section');
    soundSection.innerHTML = `
      <h3>🔊 Sound</h3>
      <label style="display:flex; align-items:center; gap:8px; font-size:13px; color:var(--ink); margin-bottom:10px; cursor:pointer;">
        <input type="checkbox" id="soundToggle" ${state.settings.soundEnabled ? 'checked' : ''}>
        Sound effects
      </label>
      <label style="display:block; font-size:12px; color:var(--ink-soft); margin-bottom:4px;">Volume</label>
      <input type="range" id="volumeSlider" min="0" max="1" step="0.05" value="${state.settings.soundVolume}" style="width:100%;">
      <button id="soundTestBtn" style="margin-top:8px; font-family:'Inter',sans-serif; font-size:12px; font-weight:600; padding:6px 12px; border-radius:8px; border:1px solid var(--border); background:var(--card); cursor:pointer;">Test sound</button>
    `;
    settingsBody.appendChild(soundSection);

    soundSection.querySelector('#soundToggle').addEventListener('change', (e) => {
      state.settings.soundEnabled = e.target.checked;
      renderAll();
    });
    soundSection.querySelector('#volumeSlider').addEventListener('input', (e) => {
      state.settings.soundVolume = parseFloat(e.target.value);
    });
    soundSection.querySelector('#volumeSlider').addEventListener('change', () => renderAll());
    soundSection.querySelector('#soundTestBtn').addEventListener('click', () => playSound('levelup'));

    // Theme
    const themeSection = document.createElement('section');
    const themeOptions = [
      { key: 'default', label: '🌱 Default' },
      { key: 'dark', label: '🌙 Dark' },
      { key: 'beer', label: '🍺 Beer' },
    ];
    themeSection.innerHTML = `
      <h3>🎨 Theme</h3>
      <div class="settings-option-row" id="themeOptionRow"></div>
    `;
    settingsBody.appendChild(themeSection);
    const themeRow = themeSection.querySelector('#themeOptionRow');
    themeOptions.forEach(opt => {
      const btn = document.createElement('button');
      btn.textContent = opt.label;
      btn.className = 'settings-option-btn' + (state.settings.theme === opt.key ? ' active' : '');
      btn.addEventListener('click', () => {
        applyTheme(opt.key);
        renderAll();
        renderSettings();
      });
      themeRow.appendChild(btn);
    });

    // Font
    const fontSection = document.createElement('section');
    const fontOptions = [
      { key: 'default', label: 'Default' },
      { key: 'serif', label: 'Serif' },
      { key: 'mono', label: 'Mono' },
      { key: 'beer', label: '🍺 Beer' },
    ];
    fontSection.innerHTML = `
      <h3>🔤 Font</h3>
      <div class="settings-option-row" id="fontOptionRow"></div>
    `;
    settingsBody.appendChild(fontSection);
    const fontRow = fontSection.querySelector('#fontOptionRow');
    fontOptions.forEach(opt => {
      const btn = document.createElement('button');
      btn.textContent = opt.label;
      btn.className = 'settings-option-btn' + (state.settings.font === opt.key ? ' active' : '');
      btn.addEventListener('click', () => {
        applyFont(opt.key);
        renderAll();
        renderSettings();
      });
      fontRow.appendChild(btn);
    });
  }

  // --- Tutorial drawer ---
  const tutorialBtn = document.getElementById('tutorialBtn');
  const tutorialPanel = document.getElementById('tutorialPanel');
  const tutorialCloseBtn = document.getElementById('tutorialCloseBtn');

  tutorialBtn.addEventListener('click', () => {
    tutorialPanel.classList.toggle('open');
  });
  tutorialCloseBtn.addEventListener('click', () => {
    tutorialPanel.classList.remove('open');
  });

  // --- Background photo picker ---
  const bgInput = document.getElementById('bgInput');
  const bgUploadBtn = document.getElementById('bgUploadBtn');
  const bgResetBtn = document.getElementById('bgResetBtn');
  const defaultBackground = document.body.style.background || getComputedStyle(document.body).backgroundImage;

  bgUploadBtn.addEventListener('click', () => bgInput.click());

  bgInput.addEventListener('change', () => {
    const file = bgInput.files[0];
    if (!file) return;
    if (!file.type.startsWith('image/')) {
      showToast('Please choose an image file');
      return;
    }
    const reader = new FileReader();
    reader.onload = (e) => {
      document.body.style.backgroundImage = `url("${e.target.result}")`;
      showToast('Background updated');
    };
    reader.onerror = () => showToast('Could not read that image');
    reader.readAsDataURL(file);
  });

  bgResetBtn.addEventListener('click', () => {
    document.body.style.backgroundImage = '';
    bgInput.value = '';
    showToast('Background reset');
  });

  // --- Rebirth panel ---
  const rebirthBtn = document.getElementById('rebirthBtn');
  const rebirthBackdrop = document.getElementById('rebirthBackdrop');
  const rebirthCloseBtn = document.getElementById('rebirthCloseBtn');
  const rebirthList = document.getElementById('rebirthList');
  let rebirthConfirmArmed = false;
  let rebirthConfirmTimer = null;

  function openRebirth() {
    rebirthConfirmArmed = false;
    renderRebirth();
    rebirthBackdrop.classList.add('open');
  }
  function closeRebirth() {
    rebirthBackdrop.classList.remove('open');
  }

  rebirthBtn.addEventListener('click', openRebirth);
  rebirthCloseBtn.addEventListener('click', closeRebirth);
  rebirthBackdrop.addEventListener('click', (e) => {
    if (e.target === rebirthBackdrop) closeRebirth();
  });

  function renderRebirth() {
    rebirthList.innerHTML = '';

    const eligible = state.level >= MIN_REBIRTH_LEVEL;
    const pointsPreview = calculateRebirthPoints();

    const summary = document.createElement('div');
    summary.className = 'quest-card';
    summary.style.cssText = 'flex-direction:column; align-items:stretch; gap:8px;';
    summary.innerHTML = `
      <div style="font-family:var(--ui-heading-font); font-weight:600; color:#6b4a1f;">
        Level ${state.level} · Rebirths: ${state.rebirths} · Rebirth Points: ${state.rebirthPoints}
      </div>
      <div style="font-size:12px; color:#8a6a3a;">
        Rebirthing resets your level, XP, coins, seeds, inventory, plots, and the entire skill tree
        back to a fresh start. It does <strong>not</strong> reset your rebirth points or anything
        bought below — those are permanent.
      </div>
      <div style="font-size:13px; font-weight:600; color:${eligible ? 'var(--leaf-dark)' : '#b23'};">
        ${eligible ? `Rebirthing now (with ${state.coins.toLocaleString()} 🪙) would earn you ${pointsPreview} rebirth point${pointsPreview === 1 ? '' : 's'} — 1 per million coins held.` : `Reach max level (${MIN_REBIRTH_LEVEL}) to unlock rebirthing — you're level ${state.level}.`}
      </div>
      <button id="rebirthConfirmBtn" ${eligible ? '' : 'disabled'} style="align-self:flex-start;">
        ${eligible ? 'Rebirth Now' : 'Locked'}
      </button>
    `;
    rebirthList.appendChild(summary);

    const confirmBtn = summary.querySelector('#rebirthConfirmBtn');
    if (eligible) {
      confirmBtn.addEventListener('click', () => {
        if (!rebirthConfirmArmed) {
          rebirthConfirmArmed = true;
          confirmBtn.textContent = 'Click again to confirm — this cannot be undone';
          confirmBtn.style.background = '#c0392b';
          clearTimeout(rebirthConfirmTimer);
          rebirthConfirmTimer = setTimeout(() => {
            rebirthConfirmArmed = false;
            if (rebirthBackdrop.classList.contains('open')) renderRebirth();
          }, 5000);
        } else {
          rebirthConfirmArmed = false;
          clearTimeout(rebirthConfirmTimer);
          performRebirth();
          renderRebirth();
        }
      });
    }

    const shopHeading = document.createElement('div');
    shopHeading.className = 'tree-column-label';
    shopHeading.style.cssText = 'margin:16px 0 8px;';
    shopHeading.textContent = '♻️ Permanent Upgrades';
    rebirthList.appendChild(shopHeading);

    Object.entries(REBIRTH_UPGRADES).forEach(([key, u]) => {
      const level = state.rebirthUpgrades[key] || 0;
      const maxed = level >= u.maxLevel;
      const cost = rebirthUpgradeCost(key);
      const card = document.createElement('div');
      card.className = 'upgrade-card' + (level > 0 ? ' owned' : '');
      card.innerHTML = `
        <div class="icon">${u.icon}</div>
        <div class="info">
          <div class="name">${u.name} <span style="color:var(--ink-soft); font-weight:500;">(Lv ${level}/${u.maxLevel})</span></div>
          <div class="desc">${u.desc}</div>
        </div>
        <button ${maxed || state.rebirthPoints < cost ? 'disabled' : ''} data-rebirth-buy="${key}">
          ${maxed ? 'Maxed' : `Buy — ${cost} ♻️`}
        </button>
      `;
      rebirthList.appendChild(card);
    });

    rebirthList.querySelectorAll('button[data-rebirth-buy]').forEach(btn => {
      btn.addEventListener('click', () => buyRebirthUpgrade(btn.getAttribute('data-rebirth-buy')));
    });
  }

</script>
</body>
</html>
