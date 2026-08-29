# Wortschatz
Wortschatz lernen B1-B2
<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Deutsch Lernboard Ab-Abonnement | Systeme.io Ready - Duden geprüft</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;700;800&family=JetBrains+Mono:wght@400;600&display=swap');
:root{--bg:#f6f7fb;--bg2:#eef1ff;--card:#ffffff;--text:#12131a;--muted:#6b7280;--primary:#5b5bf6;--primary2:#8b5cf6;--border:#e5e7eb;--shadow:0 10px 40px rgba(91,91,246,0.08);--orb1:#a5b4fc;--orb2:#f0abfc}
[data-theme="dark"]{--bg:#0a0a14;--bg2:#12122a;--card:#171732;--text:#f3f4f6;--muted:#9ca3af;--border:#23234a;--shadow:0 10px 40px rgba(0,0,0,0.4);--orb1:#4338ca;--orb2:#7e22ce}
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:'Plus Jakarta Sans',system-ui,sans-serif;background:var(--bg);color:var(--text);transition:all 0.4s ease;overflow-x:hidden}
.de-wrapper{max-width:1200px;margin:0 auto;padding:20px;position:relative}
.de-orb{position:fixed;border-radius:50%;filter:blur(80px);opacity:0.25;pointer-events:none;z-index:0}
.de-orb1{width:600px;height:600px;background:var(--orb1);top:-100px;left:-100px}
.de-orb2{width:500px;height:500px;background:var(--orb2);bottom:10%;right:-80px}
.de-header{position:relative;z-index:2;background:var(--card);border:1px solid var(--border);border-radius:24px;padding:28px;box-shadow:var(--shadow);display:flex;flex-wrap:wrap;gap:20px;justify-content:space-between;align-items:center}
.de-title{font-size:26px;font-weight:800;letter-spacing:-0.02em}
.de-title span{background:linear-gradient(90deg,var(--primary),var(--primary2));-webkit-background-clip:text;-webkit-text-fill-color:transparent}
.de-controls{display:flex;gap:12px;flex-wrap:wrap;align-items:center}
.de-search{background:var(--bg2);border:1px solid var(--border);border-radius:12px;padding:10px 16px;width:240px;color:var(--text);font-size:14px;outline:none}
.de-btn{background:var(--card);border:1px solid var(--border);border-radius:12px;padding:10px 16px;cursor:pointer;font-weight:600;font-size:14px;color:var(--text);display:flex;align-items:center;gap:8px;transition:0.2s}
.de-btn:hover{transform:translateY(-1px);border-color:var(--primary)}
.de-btn-primary{background:linear-gradient(90deg,var(--primary),var(--primary2));color:white;border:none}
.de-toggle{width:56px;height:30px;background:var(--bg2);border-radius:999px;border:1px solid var(--border);position:relative;cursor:pointer}
.de-toggle-knob{width:22px;height:22px;background:white;border-radius:50%;position:absolute;top:3px;left:3px;transition:0.3s;box-shadow:0 2px 6px rgba(0,0,0,0.2);display:flex;align-items:center;justify-content:center;font-size:12px}
[data-theme="dark"] .de-toggle-knob{transform:translateX(26px)}
.de-filters{margin:24px 0;display:flex;gap:10px;flex-wrap:wrap;z-index:2;position:relative}
.de-filter{padding:8px 16px;border-radius:999px;border:1px solid var(--border);background:var(--card);cursor:pointer;font-size:13px;font-weight:600;transition:0.2s}
.de-filter.active{background:var(--text);color:var(--bg)}
.de-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(320px,1fr));gap:20px;position:relative;z-index:2}
.de-card-wrap{perspective:1000px;height:290px}
.de-card{width:100%;height:100%;position:relative;transform-style:preserve-3d;transition:transform 0.7s cubic-bezier(0.4,0,0.2,1);cursor:pointer}
.de-card.flipped{transform:rotateY(180deg)}
.de-face{position:absolute;inset:0;backface-visibility:hidden;background:var(--card);border:1px solid var(--border);border-radius:20px;padding:22px;box-shadow:var(--shadow);display:flex;flex-direction:column;overflow:hidden}
.de-face-back{transform:rotateY(180deg)}
.de-badge{font-size:10px;letter-spacing:0.08em;text-transform:uppercase;padding:4px 10px;border-radius:999px;background:var(--bg2);border:1px solid var(--border);font-weight:700;width:fit-content}
.de-word{font-size:26px;font-weight:800;margin:12px 0 4px}
.de-phon{font-family:'JetBrains Mono',monospace;font-size:12px;color:var(--muted)}
.de-example-preview{margin-top:auto;background:var(--bg2);border-radius:12px;padding:12px;font-size:13px;line-height:1.5;border:1px dashed var(--border)}
.de-audio{width:32px;height:32px;border-radius:50%;background:var(--bg2);border:1px solid var(--border);display:inline-flex;align-items:center;justify-content:center;cursor:pointer;margin-left:8px;transition:0.2s;flex-shrink:0}
.de-audio.speaking{background:var(--primary);color:white;animation:pulse 1s infinite}
@keyframes pulse{0%,100%{transform:scale(1)}50%{transform:scale(1.1)}}
.de-back-scroll{overflow-y:auto;flex:1;margin-top:10px}
.de-ex{background:var(--bg2);border-radius:10px;padding:10px 12px;margin:8px 0;font-size:13px;line-height:1.5}
.de-ex b{color:var(--primary)}
.de-ar{font-size:12px;color:var(--muted);margin-top:4px;border-top:1px solid var(--border);padding-top:4px}
.de-hint{font-size:11px;color:var(--muted);text-align:center;margin-top:10px}
.de-quiz{margin-top:48px;position:relative;z-index:2;background:var(--card);border:1px solid var(--border);border-radius:24px;padding:32px;box-shadow:var(--shadow)}
.de-quiz-head{display:flex;justify-content:space-between;align-items:center;flex-wrap:wrap;gap:16px;margin-bottom:24px}
.de-progress{height:8px;background:var(--bg2);border-radius:999px;overflow:hidden;flex:1;max-width:300px}
.de-progress-bar{height:100%;background:linear-gradient(90deg,var(--primary),var(--primary2));transition:width 0.4s}
.de-q{background:var(--bg2);border-radius:16px;padding:20px;margin:16px 0;border:1px solid var(--border)}
.de-q-title{font-weight:700;margin-bottom:12px;line-height:1.4}
.de-options{display:grid;gap:10px}
.de-opt{padding:12px 16px;border-radius:12px;border:1px solid var(--border);background:var(--card);cursor:pointer;text-align:left;font-size:14px;transition:0.2s;color:var(--text)}
.de-opt:hover{border-color:var(--primary)}
.de-opt.correct{background:#dcfce7!important;border-color:#22c55e!important;color:#166534!important}
.de-opt.wrong{background:#fee2e2!important;border-color:#ef4444!important;color:#991b1b!important}
.de-explain{margin-top:12px;padding:12px;background:var(--card);border-radius:10px;border-left:4px solid var(--primary);font-size:13px;line-height:1.5}
.de-dropdown{position:relative}
.de-dropdown-menu{position:absolute;top:110%;right:0;background:var(--card);border:1px solid var(--border);border-radius:16px;box-shadow:var(--shadow);padding:8px;min-width:260px;z-index:10;display:none}
.de-dropdown-menu.open{display:block}
.de-drop-item{padding:10px 14px;border-radius:10px;cursor:pointer;font-size:14px;display:flex;justify-content:space-between}
.de-drop-item:hover{background:var(--bg2)}
@media(max-width:640px){.de-grid{grid-template-columns:1fr}.de-header{padding:20px}.de-title{font-size:20px}.de-search{width:100%}}
</style>
</head>
<body>
<div class="de-orb de-orb1"></div><div class="de-orb de-orb2"></div>
<div class="de-wrapper" id="de-lernboard">
<div class="de-header">
<div><div class="de-title">Deutsch <span>Lernboard</span> — Ab bis Abonnement</div><div style="font-size:12px;color:var(--muted);margin-top:4px;">Systeme.io Ready • Vanilla HTML/CSS/JS • Grammatik nach Duden geprüft • 18 Wörter</div></div>
<div class="de-controls">
<input class="de-search" id="deSearch" placeholder="Suchen: z.B. abholen..."/>
<div class="de-toggle" id="deThemeToggle" title="Tag/Nacht Modus"><div class="de-toggle-knob" id="deKnob">☀️</div></div>
<div class="de-dropdown"><button class="de-btn de-btn-primary" id="deDownloadBtn">Herunterladen ↓</button><div class="de-dropdown-menu" id="deMenu"><div class="de-drop-item" data-dl="pdf">📄 Als PDF drucken</div><div class="de-drop-item" data-dl="csv">📊 Als CSV / Excel (Anki)</div><div class="de-drop-item" data-dl="cards">🖨️ Lernkarten</div></div></div>
</div></div>
<div class="de-filters" id="deFilters"><div class="de-filter active" data-f="alle">Alle 18</div><div class="de-filter" data-f="präposition">Präpositionen</div><div class="de-filter" data-f="verb">Verben</div><div class="de-filter" data-f="nomen">Nomen</div></div>
<div class="de-grid" id="deGrid"></div>
<div class="de-quiz"><div class="de-quiz-head"><h2 style="font-size:20px;font-weight:800;">🎯 Grammatikgeprüfter Abschlusstest (Duden)</h2><div class="de-progress"><div class="de-progress-bar" id="deProg" style="width:0%"></div></div><span id="deScore" style="font-weight:700;">0 / 12</span></div><div id="deQuizContainer"></div></div>
<div style="margin-top:24px;padding:16px;background:var(--card);border:1px solid var(--border);border-radius:12px;font-size:11px;color:var(--muted);line-height:1.6;">
<strong>📦 Installation in systeme.io:</strong><br>
1. In systeme.io: Funnel → Seite bearbeiten → Element "Raw HTML" / "Code" hinzufügen<br>
2. Kopiere den gesamten Inhalt dieser Datei (Strg+A) und füge ihn in das Raw HTML Feld ein<br>
3. Speichern. Keine externen Plugins nötig. Audio funktioniert über Browser-API (de-DE).<br>
4. Für reine Karten ohne Header/Footer: kopiere nur &lt;div id="de-lernboard"&gt;...&lt;/div&gt; + &lt;style&gt; + &lt;script&gt;
</div>
</div>
<script>
const vocab=[
{id:'ab',word:'ab',type:'präposition',badge:'Präposition + Dativ',phon:'/ap/',front:'Startpunkt: ab Ort/Zeit',examples:[{de:'Die Fahrt kostet <b>ab</b> Hamburg 200 Euro.',ar:'الرحلة ابتداءً من هامبورغ 200 يورو.',note:'ab + Dativ: Ausgangspunkt'},{de:'<b>Ab</b> nächster Woche bleibt unser Geschäft samstags geschlossen.',ar:'ابتداءً من الأسبوع القادم متجرنا مغلق السبت.',note:'ab + Zeit = ab diesem Zeitpunkt'},{de:'Mein Bruder besucht uns <b>ab und zu</b>.',ar:'أخي يزورنا من حين لآخر.',note:'Feste Wendung = manchmal'}]},
{id:'abbiegen',word:'abbiegen',type:'verb',badge:'trennbares Verb',phon:'/ˈapˌbiːɡn̩/',conj:'biegt ab, bog ab, ist abgebogen',front:'Richtung ändern',examples:[{de:'An der nächsten Kreuzung müssen Sie links <b>abbiegen</b>.',ar:'في التقاطع القادم يجب أن تنعطف يساراً.',note:'Trennbar: er biegt ab, Modalverb + Infinitiv am Ende'}]},
{id:'abbildung',word:'die Abbildung',type:'nomen',badge:'Nomen -en',phon:'/ˈapˌbɪldʊŋ/',front:'Bild im Text',examples:[{de:'Hier in der <b>Abbildung</b> sehen Sie, wie man das Gerät einschaltet.',ar:'هنا في الصورة ترى كيف تشغل الجهاز.',note:'Feminin, Plural: Abbildungen, Dativ: in der Abbildung'}]},
{id:'aber',word:'aber',type:'präposition',badge:'Konjunktion',phon:'/ˈaːbɐ/',front:'Gegensatz & Zustimmung',examples:[{de:'Heute kann ich nicht, <b>aber</b> morgen ganz bestimmt.',ar:'اليوم لا أستطيع، لكن غداً بالتأكيد.',note:'Konjunktion, Komma davor'},{de:'Es lag sehr viel Schnee, <b>aber</b> Enzo ist trotzdem mit dem Motorrad gefahren.',ar:'ثلج كثير، لكن إنزو قاد الدراجة.',note:'trotzdem verstärkt Gegensatz'},{de:'Wir haben nur eine kleine Wohnung, sind <b>aber</b> damit zufrieden.',ar:'شقة صغيرة لكننا راضون.',note:'aber als Adverb Position 1 nach Komma'},{de:'Es war sehr schön. Jetzt muss ich <b>aber</b> gehen.',ar:'كان جميلاً، لكن يجب أن أذهب.',note:'Modalpartikel: Bedauern'},{de:'Aber ja, sehr gern!',ar:'نعم بالطبع بكل سرور!',note:'Verstärkte Zustimmung'}]},
{id:'abfall',word:'der Abfall',type:'nomen',badge:'Nomen -¨e',phon:'/ˈapfal/',front:'Müll',examples:[{de:'Werfen Sie den Bio<b>abfall</b> in die grüne Tonne.',ar:'ارمِ النفايات العضوية في الحاوية الخضراء.',note:'Kompositum Bio+Abfall, Pl: Abfälle'}]},
{id:'abfahren',word:'abfahren',type:'verb',badge:'trennbares Verb',phon:'/ˈapˌfaːʁən/',conj:'fährt ab, fuhr ab, ist abgefahren',front:'losfahren',examples:[{de:'Unser Zug ist pünktlich <b>abgefahren</b>.',ar:'قطارنا انطلق في موعده.',note:'Perfekt mit sein (Bewegung)'}]},
{id:'abgas',word:'das Abgas',type:'nomen',badge:'Nomen -e (Pl.)',phon:'/ˈapɡaːs/',front:'Auspuffgas',examples:[{de:'<b>Abgase</b> aus Industrie und Haushalten verschmutzen die Luft.',ar:'غازات العادم تلوث الهواء.',note:'Nur Plural üblich: die Abgase'}]},
{id:'abgeben',word:'abgeben',type:'verb',badge:'trennbares Verb',phon:'/ˈapˌɡeːbn̩/',conj:'gibt ab, gab ab, hat abgegeben',front:'übergeben',examples:[{de:'Ich soll dieses Päckchen bei Herrn Müller <b>abgeben</b>.',ar:'يجب أن أسلم الطرد عند السيد مولر.',note:'bei + Dativ'}]},
{id:'abhaengen',word:'abhängen',type:'verb',badge:'trennbares Verb',phon:'/ˈapˌhɛŋən/',conj:'hängt ab, hing ab, hat abgehangen',front:'abhängig sein',examples:[{de:'Vielleicht bleiben wir länger, das hängt vom Wetter <b>ab</b>.',ar:'ربما نبقى أطول، هذا يعتمد على الطقس.',note:'hängt ab von + Dativ, Präfix am Ende'}]},
{id:'abhaengig',word:'abhängig',type:'präposition',badge:'Adjektiv',phon:'/ˈapˌhɛŋɪç/',front:'nicht selbstständig',examples:[{de:'Gregor ist finanziell von seinen Eltern <b>abhängig</b>.',ar:'غريغور معتمد مالياً على والديه.',note:'abhängig von + Dativ'}]},
{id:'abheben',word:'abheben',type:'verb',badge:'trennbares Verb',phon:'/ˈapˌheːbn̩/',conj:'hebt ab, hob ab, hat abgehoben',front:'Geld abheben',examples:[{de:'Für die Reise habe ich 500 Euro von meinem Konto <b>abgehoben</b>.',ar:'سحبت 500 يورو من حسابي للرحلة.',note:'von + Dativ'}]},
{id:'abholen',word:'abholen',type:'verb',badge:'trennbares Verb',phon:'/ˈapˌhoːlən/',conj:'holt ab, holte ab, hat abgeholt',front:'jemanden abholen',examples:[{de:'Meine Freundin hat mich vom Bahnhof <b>abgeholt</b>.',ar:'صديقتي أخذتني من المحطة.',note:'hat abgeholt, von = vom'}]},
{id:'abitur',word:'das Abitur',type:'nomen',badge:'Nomen',phon:'/abiˈtuːɐ/',front:'Schulabschluss',examples:[{de:'Meine Tochter hat gerade <b>Abitur</b> gemacht.',ar:'ابنتي حصلت على الثانوية للتو.',note:'Feste Wendung: Abitur machen'}]},
{id:'ablehnen',word:'ablehnen',type:'verb',badge:'trennbares Verb',phon:'/ˈapˌleːnən/',conj:'lehnt ab, lehnte ab, hat abgelehnt',front:'verneinen',examples:[{de:'Es tut mir leid, Ihr Antrag ist <b>abgelehnt</b>.',ar:'آسف، طلبك مرفوض.',note:'Zustandspassiv: ist abgelehnt'}]},
{id:'abmachen',word:'abmachen',type:'verb',badge:'trennbares Verb',phon:'/ˈapˌmaxn̩/',conj:'macht ab, machte ab, hat abgemacht',front:'vereinbaren',examples:[{de:'Wir hatten doch <b>abgemacht</b>, dass du die Getränke besorgst.',ar:'اتفقنا أنك تحضر المشروبات.',note:'+ dass-Satz, umgangssprachlich'}]},
{id:'abnehmen',word:'abnehmen',type:'verb',badge:'trennbares Verb',phon:'/ˈapˌneːmən/',conj:'nimmt ab, nahm ab, hat abgenommen',front:'entfernen / abnehmen',examples:[{de:'Morgen können wir den Verband <b>abnehmen</b>.',ar:'غداً نزيل الضمادة.',note:'Bedeutung 1: entfernen + Akk'},{de:'Ich habe zehn Kilo <b>abgenommen</b>.',ar:'فقدت عشرة كيلو.',note:'Bedeutung 2: Gewicht verlieren'}]},
{id:'abonnieren',word:'abonnieren',type:'verb',badge:'Verb',phon:'/abɔˈniːʁən/',conj:'abonniert, abonnierte, hat abonniert',front:'regelmäßig beziehen',examples:[{de:'Diese Zeitschrift würde ich gerne <b>abonnieren</b>.',ar:'أود الاشتراك في هذه المجلة.',note:'Konjunktiv II: würde ... = höflich'}]},
{id:'abonnement',word:'das Abonnement',type:'nomen',badge:'Nomen -s',phon:'/abɔnəˈmɑ̃ː/',front:'Abo',examples:[{de:'Ich habe das <b>Abonnement</b> gekündigt.',ar:'ألغيت الاشتراك.',note:'Pl: Abonnements, kündigen = beenden'}]},
];
function speak(t){if(!('speechSynthesis' in window))return;window.speechSynthesis.cancel();const c=t.replace(/<[^>]*>/g,'');const u=new SpeechSynthesisUtterance(c);u.lang='de-DE';u.rate=0.85;const vs=speechSynthesis.getVoices();const dv=vs.find(v=>v.lang.startsWith('de'));if(dv)u.voice=dv;speechSynthesis.speak(u);return u;}
function renderGrid(f='alle',s=''){const g=document.getElementById('deGrid');g.innerHTML='';vocab.filter(v=>{const fm=f==='alle'||v.type===f;const sm=!s||(v.word.toLowerCase().includes(s.toLowerCase())||v.front.toLowerCase().includes(s.toLowerCase()));return fm&&sm;}).forEach(v=>{const w=document.createElement('div');w.className='de-card-wrap';w.innerHTML=`<div class="de-card" data-id="${v.id}"><div class="de-face"><div style="display:flex;justify-content:space-between;"><div class="de-badge">${v.badge}</div><button class="de-audio" data-speak="${v.word}">🔊</button></div><div class="de-word">${v.word}</div><div class="de-phon">${v.phon} ${v.conj?'• '+v.conj:''}</div><div style="margin-top:6px;font-size:13px;color:var(--muted)">${v.front}</div><div class="de-example-preview">${v.examples[0].de}</div><div class="de-hint">Klicken zum Drehen ↻ — ${v.examples.length} Bsp.</div></div><div class="de-face de-face-back"><div style="display:flex;justify-content:space-between;"><div class="de-badge">${v.badge}</div><span style="font-size:11px;color:var(--muted)">↺ zurück</span></div><div class="de-back-scroll">${v.examples.map(ex=>`<div class="de-ex"><div style="display:flex;justify-content:space-between;gap:8px;"><span>${ex.de}</span><button class="de-audio" data-speak="${ex.de}">🔊</button></div><div class="de-ar">🇸🇦 ${ex.ar}<br>💡 ${ex.note}</div></div>`).join('')}</div></div></div>`;g.appendChild(w);});attach();}
function attach(){document.querySelectorAll('.de-card').forEach(c=>{c.addEventListener('click',e=>{if(e.target.closest('.de-audio'))return;c.classList.toggle('flipped');});});document.querySelectorAll('.de-audio').forEach(b=>{b.addEventListener('click',e=>{e.stopPropagation();const t=b.getAttribute('data-speak');document.querySelectorAll('.de-audio').forEach(x=>x.classList.remove('speaking'));b.classList.add('speaking');const u=speak(t);if(u){u.onend=()=>b.classList.remove('speaking');}else setTimeout(()=>b.classList.remove('speaking'),1500);});});}
document.getElementById('deFilters').addEventListener('click',e=>{if(!e.target.classList.contains('de-filter'))return;document.querySelectorAll('.de-filter').forEach(f=>f.classList.remove('active'));e.target.classList.add('active');renderGrid(e.target.dataset.f,document.getElementById('deSearch').value);});
document.getElementById('deSearch').addEventListener('input',e=>{const a=document.querySelector('.de-filter.active').dataset.f;renderGrid(a,e.target.value);});
const tog=document.getElementById('deThemeToggle');const knob=document.getElementById('deKnob');function setTheme(t){document.documentElement.setAttribute('data-theme',t);localStorage.setItem('de-theme',t);knob.textContent=t==='dark'?'🌙':'☀️';}setTheme(localStorage.getItem('de-theme')||'light');tog.addEventListener('click',()=>{const c=document.documentElement.getAttribute('data-theme');setTheme(c==='dark'?'light':'dark');});
const dlBtn=document.getElementById('deDownloadBtn');const menu=document.getElementById('deMenu');dlBtn.addEventListener('click',()=>menu.classList.toggle('open'));document.addEventListener('click',e=>{if(!e.target.closest('.de-dropdown'))menu.classList.remove('open');});menu.addEventListener('click',e=>{const it=e.target.closest('.de-drop-item');if(!it)return;const ty=it.dataset.dl;if(ty==='pdf'||ty==='cards'){const win=window.open('','_blank');const rows=vocab.map(v=>`<tr><td><b>${v.word}</b><br><small>${v.badge} ${v.conj||''}</small></td><td>${v.examples.map(ex=>ex.de).join('<br>')}</td><td>${v.examples.map(ex=>ex.ar).join('<br>')}</td></tr>`).join('');win.document.write(`<html><head><meta charset="utf-8"><title>Deutsch Lernboard</title><style>body{font-family:Arial;padding:20px}table{width:100%;border-collapse:collapse}th,td{border:1px solid #ddd;padding:8px;font-size:12px}th{background:#5b5bf6;color:white}</style></head><body><h1>Deutsch Lernboard Ab-Abonnement</h1><p>Duden geprüft • ${new Date().toLocaleDateString('de-DE')}</p><table><tr><th>Wort</th><th>Deutsch</th><th>Arabisch</th></tr>${rows}</table><script>window.print()<\\/script></body></html>`);win.document.close();}if(ty==='csv'){let csv="Wort;Wortart;Konjugation;Beispiel;Bedeutung;Arabisch;Hinweis\n";vocab.forEach(v=>{v.examples.forEach(ex=>{const cd=ex.de.replace(/<[^>]*>/g,'').replace(/;/g,',');csv+=`${v.word};${v.badge};${v.conj||''};${cd};${v.front};${ex.ar};${ex.note}\n`;});});const blob=new Blob([csv],{type:'text/csv;charset=utf-8;'});const url=URL.createObjectURL(blob);const a=document.createElement('a');a.href=url;a.download='deutsch_ab_abonnement_duden.csv';a.click();}menu.classList.remove('open');});
const quizData=[{q:'Die Fahrt kostet ___ Hamburg 200 Euro. (Startpunkt)',opts:['ab','an','auf'],correct:0,explain:'Korrekt: <b>ab Hamburg</b> – Präposition <b>ab</b> + Dativ für Ausgangspunkt.'},{q:'An der nächsten Kreuzung müssen Sie links ___.',opts:['abbiegen','abgeben','abholen'],correct:0,explain:'Korrekt: <b>abbiegen</b> – trennbar. Mit Modalverb Infinitiv am Ende: müssen ... abbiegen. Perfekt: ist <b>abgebogen</b>.'},{q:'Hier in der ___ sehen Sie die Anleitung.',opts:['Abbildung','Abfall','Abgas'],correct:0,explain:'Korrekt: <b>die Abbildung, -en</b> – feminin, Dativ: in der Abbildung.'},{q:'Heute kann ich nicht, ___ morgen ganz bestimmt.',opts:['aber','ab','ob'],correct:0,explain:'Korrekt: <b>aber</b> Konjunktion, Komma davor! Gegensatz.'},{q:'Werfen Sie den Bioabfall in die ___ Tonne.',opts:['grüne','grün','grünen'],correct:0,explain:'Korrekt: <b>grüne</b> – Adjektiv: die grüne Tonne (Nom. fem. schwach nach definitem Artikel).'},{q:'Unser Zug ist pünktlich ___.',opts:['abgefahren','abgegeben','abgeholt'],correct:0,explain:'Korrekt: <b>abgefahren</b> – Perfekt mit sein: ist abgefahren (Bewegung).'},{q:'___ aus Fabriken verschmutzen die Luft.',opts:['Abgase','Abfälle','Abbildungen'],correct:0,explain:'Korrekt: <b>Abgase</b> – nur Plural üblich: die Abgase.'},{q:'Ich soll das Päckchen bei Herrn Müller ___.',opts:['abgeben','abheben','abhängen'],correct:0,explain:'Korrekt: <b>abgeben bei + Dativ</b> = dort übergeben.'},{q:'Das hängt vom Wetter ___.',opts:['ab','an','auf'],correct:0,explain:'Korrekt: <b>abhängen von + Dativ</b> – trennbar: hängt ... ab (Präfix am Ende).'},{q:'Meine Freundin hat mich vom Bahnhof ___.',opts:['abgeholt','abgefahren','abgenommen'],correct:0,explain:'Korrekt: <b>abgeholt</b> – Perfekt: hat abgeholt. vom = von dem (Dativ).'},{q:'Ich habe zehn Kilo ___.',opts:['abgenommen','abgemacht','abgelehnt'],correct:0,explain:'Korrekt: <b>abgenommen</b> – 2 Bedeutungen: Verband entfernen / Gewicht verlieren.'},{q:'Ich habe das Abonnement ___.',opts:['gekündigt','abonniert','abgeholt'],correct:0,explain:'Korrekt: <b>gekündigt</b> – kündigen = beenden, abonnieren = beginnen.'},];
let score=0,answered=0;function renderQuiz(){const cont=document.getElementById('deQuizContainer');cont.innerHTML='';quizData.forEach((it,i)=>{const d=document.createElement('div');d.className='de-q';d.innerHTML=`<div class="de-q-title">${i+1}. ${it.q}</div><div class="de-options">${it.opts.map((o,j)=>`<button class="de-opt" data-q="${i}" data-o="${j}">${o}</button>`).join('')}</div><div class="de-explain" id="exp-${i}" style="display:none"></div>`;cont.appendChild(d);});cont.addEventListener('click',e=>{if(!e.target.classList.contains('de-opt'))return;const qi=parseInt(e.target.dataset.q);const oi=parseInt(e.target.dataset.o);const qd=e.target.closest('.de-q');if(qd.dataset.done)return;qd.dataset.done='1';const cor=quizData[qi].correct;qd.querySelectorAll('.de-opt').forEach((op,j)=>{if(j===cor)op.classList.add('correct');else if(j===oi&&oi!==cor)op.classList.add('wrong');op.style.pointerEvents='none';});const ex=document.getElementById(`exp-${qi}`);ex.style.display='block';ex.innerHTML=(oi===cor?'✅ <b>Richtig!</b> ':'❌ <b>Falsch.</b> ')+quizData[qi].explain;if(oi===cor)score++;answered++;document.getElementById('deScore').textContent=`${score} / ${quizData.length}`;document.getElementById('deProg').style.width=`${(answered/quizData.length)*100}%`;if(answered===quizData.length){setTimeout(()=>{const r=document.createElement('div');r.style.cssText='margin-top:20px;padding:20px;background:linear-gradient(90deg,var(--primary),var(--primary2));color:white;border-radius:16px;text-align:center';r.innerHTML=`<h3>🎉 Test beendet!</h3><p style="font-size:28px;font-weight:800;margin:10px 0">${score} / ${quizData.length}</p><p>${score>=10?'Ausgezeichnet! Duden-Niveau!':score>=7?'Gut! Noch einmal wiederholen.':'Übe die Karten!'}</p><button class="de-btn" style="margin:12px auto 0;background:white;color:#5b5bf6" onclick="location.reload()">Nochmal ↻</button>`;cont.appendChild(r);},400);}});}
renderGrid();renderQuiz();if('speechSynthesis' in window)speechSynthesis.getVoices();
</script>
</body>
</html>
