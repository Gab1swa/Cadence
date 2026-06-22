import React, { useState, useEffect, useRef } from "react";
import {
  Sparkles, Lightbulb, FileText, Film, Settings as SettingsIcon,
  Plus, Search, Copy, Trash2, Wand2, LayoutDashboard, Clock,
  Check, ArrowRight, Pencil, X, Loader2, TrendingUp, Hash, Zap
} from "lucide-react";

/* ------------------------------------------------------------------ */
/*  Design system (brief: Montserrat, fond #050505, halos, glass)     */
/* ------------------------------------------------------------------ */
const STYLES = `
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700;800&display=swap');

* { box-sizing: border-box; }
.cad-root {
  font-family: 'Montserrat', system-ui, sans-serif;
  background: #050505;
  color: #f2f2f2;
  min-height: 100vh;
  position: relative;
  overflow-x: hidden;
  letter-spacing: 0.1px;
}
.cad-root::before {
  content: '';
  position: fixed; inset: 0;
  background:
    radial-gradient(620px circle at 12% 8%, rgba(255,255,255,0.055), transparent 48%),
    radial-gradient(520px circle at 88% 28%, rgba(255,255,255,0.035), transparent 50%),
    radial-gradient(760px circle at 72% 96%, rgba(255,255,255,0.045), transparent 55%);
  pointer-events: none; z-index: 0;
}
.cad-shell { position: relative; z-index: 1; max-width: 1180px; margin: 0 auto; padding: 0 22px 80px; }

.glass {
  background: rgba(255,255,255,0.04);
  backdrop-filter: blur(18px) saturate(120%);
  -webkit-backdrop-filter: blur(18px) saturate(120%);
  border: 1px solid rgba(255,255,255,0.10);
  border-radius: 20px;
  box-shadow: 0 22px 55px -16px rgba(0,0,0,0.75);
}
.glass-hover { transition: transform .5s cubic-bezier(0.25,0.8,0.25,1), box-shadow .5s cubic-bezier(0.25,0.8,0.25,1), border-color .5s cubic-bezier(0.25,0.8,0.25,1); }
.glass-hover:hover {
  transform: translateY(-6px);
  border-color: rgba(255,255,255,0.22);
  box-shadow: 0 34px 70px -14px rgba(0,0,0,0.85), 0 0 34px rgba(255,255,255,0.09);
}
.ic { transition: transform .5s cubic-bezier(0.25,0.8,0.25,1); }
.glass-hover:hover .ic, .nav-btn:hover .ic, .btn:hover .ic { transform: scale(1.18); }

.btn {
  font-family: inherit; cursor: pointer; border-radius: 14px;
  display: inline-flex; align-items: center; gap: 9px; justify-content: center;
  font-weight: 600; font-size: 14px; letter-spacing: .2px;
  transition: transform .5s cubic-bezier(0.25,0.8,0.25,1), box-shadow .5s cubic-bezier(0.25,0.8,0.25,1), background .35s, border-color .35s, opacity .3s;
}
.btn-primary { background: #f2f2f2; color: #050505; border: 1px solid #fff; padding: 12px 20px; }
.btn-primary:hover { transform: translateY(-3px); box-shadow: 0 16px 34px -10px rgba(255,255,255,0.35); }
.btn-ghost { background: rgba(255,255,255,0.05); color: #f2f2f2; border: 1px solid rgba(255,255,255,0.12); padding: 11px 16px; }
.btn-ghost:hover { transform: translateY(-3px); border-color: rgba(255,255,255,0.3); box-shadow: 0 0 24px rgba(255,255,255,0.07); }
.btn-icon { background: rgba(255,255,255,0.04); border: 1px solid rgba(255,255,255,0.1); color: #cfcfcf; padding: 9px; border-radius: 12px; cursor: pointer; transition: all .4s cubic-bezier(0.25,0.8,0.25,1); }
.btn-icon:hover { color: #fff; border-color: rgba(255,255,255,0.3); transform: translateY(-2px); box-shadow: 0 0 18px rgba(255,255,255,0.08); }
.btn:disabled { opacity: .45; cursor: not-allowed; transform: none !important; box-shadow: none !important; }

.field {
  width: 100%; font-family: inherit; font-size: 14px; color: #f2f2f2;
  background: rgba(0,0,0,0.35); border: 1px solid rgba(255,255,255,0.12);
  border-radius: 14px; padding: 13px 15px; outline: none;
  transition: border-color .35s, box-shadow .35s;
}
.field:focus { border-color: rgba(255,255,255,0.4); box-shadow: 0 0 0 3px rgba(255,255,255,0.06); }
.field::placeholder { color: #777; }
textarea.field { resize: vertical; line-height: 1.55; }
select.field { appearance: none; cursor: pointer; }

.nav-btn {
  display: inline-flex; align-items: center; gap: 9px; cursor: pointer;
  font-family: inherit; font-weight: 600; font-size: 13.5px; letter-spacing: .3px;
  padding: 11px 16px; border-radius: 14px; border: 1px solid transparent;
  background: transparent; color: #8a8a8a;
  transition: all .45s cubic-bezier(0.25,0.8,0.25,1);
}
.nav-btn:hover { color: #f2f2f2; background: rgba(255,255,255,0.04); }
.nav-btn.active { color: #050505; background: #f2f2f2; border-color: #fff; }

.chip {
  font-size: 11px; font-weight: 600; letter-spacing: .5px; text-transform: uppercase;
  padding: 5px 11px; border-radius: 999px; border: 1px solid rgba(255,255,255,0.14);
  background: rgba(255,255,255,0.05); color: #bfbfbf;
}
.tag {
  font-size: 11px; padding: 3px 9px; border-radius: 8px;
  background: rgba(255,255,255,0.06); border: 1px solid rgba(255,255,255,0.1); color: #c9c9c9;
}
.fade-in { animation: fadeUp .55s cubic-bezier(0.25,0.8,0.25,1) both; }
@keyframes fadeUp { from { opacity: 0; transform: translateY(14px); } to { opacity: 1; transform: none; } }
.spin { animation: spin 1s linear infinite; }
@keyframes spin { to { transform: rotate(360deg); } }

.grid-cards { display: grid; gap: 16px; }
.label-eyebrow { font-size: 11px; letter-spacing: 2px; text-transform: uppercase; color: #6e6e6e; font-weight: 600; }
.muted { color: #8a8a8a; }
.hr { height: 1px; background: rgba(255,255,255,0.08); border: 0; margin: 0; }
a, a:visited { color: #fff; }

@media (prefers-reduced-motion: reduce) {
  *, .glass-hover, .btn, .ic, .nav-btn, .fade-in { transition: none !important; animation: none !important; }
}
@media (max-width: 640px){
  .cad-shell { padding: 0 14px 70px; }
}
`;

/* ------------------------------------------------------------------ */
/*  Helpers                                                            */
/* ------------------------------------------------------------------ */
const uid = () => Date.now().toString(36) + Math.random().toString(36).slice(2, 7);
const STORE_KEY = "cadence:data:v1";
const STATUSES = ["idée", "à scripter", "scriptée", "tournée", "publiée"];
const PLATFORMS = ["TikTok", "Instagram Reels", "YouTube Shorts", "Multi-plateforme"];
const TONES = ["Dynamique et direct", "Pédagogique et clair", "Storytelling immersif", "Drôle et décalé", "Premium et posé", "Provocateur"];
const DURATIONS = ["15–30 s", "30–60 s", "60–90 s"];

const DEFAULT_DATA = {
  ideas: [],
  videos: [],
  settings: { niche: "", audience: "", tone: TONES[0], defaultPlatform: "TikTok", ideaCount: 5 },
};

function extractJSON(text) {
  if (!text) throw new Error("Réponse vide");
  let t = text.trim().replace(/```json/gi, "").replace(/```/g, "").trim();
  const fo = t.indexOf("{"), fa = t.indexOf("[");
  let start, close;
  if (fa !== -1 && (fo === -1 || fa < fo)) { start = fa; close = "]"; }
  else { start = fo; close = "}"; }
  if (start === -1) throw new Error("Pas de JSON détecté");
  const end = t.lastIndexOf(close);
  return JSON.parse(t.slice(start, end + 1));
}

async function callClaude(system, user) {
  const res = await fetch("https://api.anthropic.com/v1/messages", {
    method: "POST",
    headers: { "Content-Type": "application/json" },
    body: JSON.stringify({
      model: "claude-sonnet-4-6",
      max_tokens: 1000,
      system,
      messages: [{ role: "user", content: user }],
    }),
  });
  if (!res.ok) throw new Error("Le service IA a renvoyé une erreur (" + res.status + ").");
  const data = await res.json();
  return (data.content || []).map((b) => (b.type === "text" ? b.text : "")).join("\n");
}

function buildContext(data) {
  const s = data.settings;
  let c = `Thématique de la chaîne : ${s.niche || "non précisée"}\n`;
  c += `Audience visée : ${s.audience || "non précisée"}\n`;
  c += `Ton de marque souhaité : ${s.tone}\n`;
  if (data.videos.length) {
    c += `\nVidéos déjà publiées (récentes en premier) :\n`;
    data.videos.slice(0, 12).forEach((v) => {
      c += `- « ${v.title} » | thème : ${v.theme || "?"} | ${v.platform} | perf : ${v.performance || "?"} | ce qui a marché : ${v.worked || "?"}\n`;
    });
  }
  if (data.ideas.length) {
    c += `\nIdées et notes en cours :\n`;
    data.ideas.slice(0, 15).forEach((i) => {
      c += `- ${i.title}${i.notes ? " — " + i.notes.slice(0, 120) : ""}\n`;
    });
  }
  return c;
}

/* ------------------------------------------------------------------ */
/*  App                                                                */
/* ------------------------------------------------------------------ */
export default function App() {
  const [data, setData] = useState(DEFAULT_DATA);
  const [loaded, setLoaded] = useState(false);
  const [tab, setTab] = useState("dashboard");
  const [toast, setToast] = useState(null);
  const [studioIdeaId, setStudioIdeaId] = useState(null);
  const saveTimer = useRef(null);

  // Load once
  useEffect(() => {
    (async () => {
      try {
        const r = await window.storage.get(STORE_KEY);
        if (r && r.value) setData({ ...DEFAULT_DATA, ...JSON.parse(r.value) });
      } catch (_) { /* première utilisation */ }
      setLoaded(true);
    })();
  }, []);

  // Persist (debounced)
  useEffect(() => {
    if (!loaded) return;
    clearTimeout(saveTimer.current);
    saveTimer.current = setTimeout(async () => {
      try { await window.storage.set(STORE_KEY, JSON.stringify(data)); } catch (_) {}
    }, 500);
  }, [data, loaded]);

  const notify = (msg) => { setToast(msg); setTimeout(() => setToast(null), 2600); };
  const update = (patch) => setData((d) => ({ ...d, ...patch }));

  const openStudioWith = (id) => { setStudioIdeaId(id); setTab("studio"); };

  const NAV = [
    { id: "dashboard", label: "Tableau de bord", Icon: LayoutDashboard },
    { id: "ideas", label: "Idées", Icon: Lightbulb },
    { id: "studio", label: "Studio script", Icon: FileText },
    { id: "library", label: "Bibliothèque", Icon: Film },
    { id: "settings", label: "Réglages", Icon: SettingsIcon },
  ];

  if (!loaded) {
    return (
      <div className="cad-root">
        <style>{STYLES}</style>
        <div style={{ display: "flex", height: "100vh", alignItems: "center", justifyContent: "center", gap: 12 }}>
          <Loader2 size={20} className="spin" /> <span className="muted">Chargement de ton studio…</span>
        </div>
      </div>
    );
  }

  return (
    <div className="cad-root">
      <style>{STYLES}</style>
      <div className="cad-shell">
        {/* Header */}
        <header style={{ padding: "30px 0 22px", display: "flex", flexWrap: "wrap", gap: 16, alignItems: "center", justifyContent: "space-between" }}>
          <div>
            <div style={{ display: "flex", alignItems: "center", gap: 12 }}>
              <div className="glass" style={{ width: 42, height: 42, borderRadius: 14, display: "grid", placeItems: "center" }}>
                <Zap size={20} />
              </div>
              <div>
                <div style={{ fontWeight: 800, fontSize: 22, letterSpacing: 3 }}>CADENCE</div>
                <div className="label-eyebrow" style={{ marginTop: 2 }}>Studio vidéo · format court</div>
              </div>
            </div>
          </div>
          <nav style={{ display: "flex", gap: 6, flexWrap: "wrap" }}>
            {NAV.map(({ id, label, Icon }) => (
              <button key={id} className={"nav-btn" + (tab === id ? " active" : "")} onClick={() => setTab(id)}>
                <Icon size={16} className="ic" /> {label}
              </button>
            ))}
          </nav>
        </header>

        <main key={tab} className="fade-in">
          {tab === "dashboard" && <Dashboard data={data} update={update} notify={notify} openStudioWith={openStudioWith} setTab={setTab} />}
          {tab === "ideas" && <Ideas data={data} update={update} notify={notify} openStudioWith={openStudioWith} />}
          {tab === "studio" && <Studio data={data} update={update} notify={notify} studioIdeaId={studioIdeaId} setStudioIdeaId={setStudioIdeaId} />}
          {tab === "library" && <Library data={data} update={update} notify={notify} />}
          {tab === "settings" && <SettingsView data={data} update={update} notify={notify} />}
        </main>
      </div>

      {toast && (
        <div className="glass fade-in" style={{ position: "fixed", bottom: 26, left: "50%", transform: "translateX(-50%)", padding: "13px 22px", zIndex: 50, display: "flex", gap: 9, alignItems: "center", fontSize: 14, fontWeight: 600 }}>
          <Check size={16} /> {toast}
        </div>
      )}
    </div>
  );
}

/* ------------------------------------------------------------------ */
/*  Dashboard                                                          */
/* ------------------------------------------------------------------ */
function Dashboard({ data, update, notify, openStudioWith, setTab }) {
  const [quick, setQuick] = useState("");
  const [loadingIdeas, setLoadingIdeas] = useState(false);
  const [suggestions, setSuggestions] = useState([]);
  const [err, setErr] = useState("");

  const stats = [
    { label: "Idées", value: data.ideas.length, Icon: Lightbulb },
    { label: "Scriptées", value: data.ideas.filter((i) => i.script).length, Icon: FileText },
    { label: "Publiées", value: data.videos.length, Icon: Film },
  ];

  const addQuick = () => {
    const t = quick.trim();
    if (!t) return;
    const idea = { id: uid(), title: t.split("\n")[0].slice(0, 80), notes: t, tags: [], status: "idée", platform: data.settings.defaultPlatform, createdAt: Date.now(), script: null };
    update({ ideas: [idea, ...data.ideas] });
    setQuick("");
    notify("Idée enregistrée");
  };

  const genIdeas = async () => {
    setErr(""); setLoadingIdeas(true); setSuggestions([]);
    try {
      const n = data.settings.ideaCount || 5;
      const system = "Tu es un stratège de contenu expert en vidéos format court (TikTok, Reels, Shorts). Tu raisonnes à partir des données réelles du créateur. Tu réponds toujours en français et UNIQUEMENT en JSON valide, sans texte ni balises autour.";
      const user = `${buildContext(data)}\n\nPropose ${n} idées de vidéos NOUVELLES et concrètes qui exploitent ce qui fonctionne déjà et prolongent les notes ci-dessus, sans répéter les vidéos publiées. Pour chaque idée : un titre accrocheur, l'angle, un hook (1 phrase prête à dire), et pourquoi ça peut marcher pour cette audience.\nFormat de réponse JSON strict : [{"title":"","angle":"","hook":"","why":""}]`;
      const txt = await callClaude(system, user);
      const arr = extractJSON(txt);
      setSuggestions(Array.isArray(arr) ? arr : []);
    } catch (e) {
      setErr("Génération impossible pour le moment. Réessaie dans un instant.");
    } finally { setLoadingIdeas(false); }
  };

  const adoptIdea = (s) => {
    const idea = { id: uid(), title: s.title, notes: [s.angle, s.hook ? "Hook : " + s.hook : "", s.why ? "Pourquoi : " + s.why : ""].filter(Boolean).join("\n"), tags: ["IA"], status: "à scripter", platform: data.settings.defaultPlatform, createdAt: Date.now(), script: null };
    update({ ideas: [idea, ...data.ideas] });
    setSuggestions((prev) => prev.filter((x) => x !== s));
    notify("Ajoutée à tes idées");
  };

  return (
    <div className="grid-cards" style={{ gridTemplateColumns: "1fr" }}>
      {/* Quick capture */}
      <section className="glass glass-hover" style={{ padding: 24 }}>
        <div style={{ display: "flex", alignItems: "center", gap: 10, marginBottom: 14 }}>
          <Sparkles size={18} className="ic" />
          <h2 style={{ margin: 0, fontSize: 17, fontWeight: 700 }}>Capture rapide</h2>
        </div>
        <p className="muted" style={{ margin: "0 0 14px", fontSize: 13.5 }}>Une idée qui passe ? Note-la ici, l'IA s'en servira pour le reste.</p>
        <textarea className="field" rows={3} placeholder="Ex : tuto montage 30 s, erreur que tout le monde fait au démarrage…" value={quick} onChange={(e) => setQuick(e.target.value)} />
        <div style={{ marginTop: 12 }}>
          <button className="btn btn-primary" onClick={addQuick} disabled={!quick.trim()}><Plus size={16} className="ic" /> Enregistrer l'idée</button>
        </div>
      </section>

      {/* Stats */}
      <div className="grid-cards" style={{ gridTemplateColumns: "repeat(auto-fit, minmax(150px, 1fr))" }}>
        {stats.map(({ label, value, Icon }) => (
          <div key={label} className="glass glass-hover" style={{ padding: 22 }}>
            <Icon size={18} className="ic muted" />
            <div style={{ fontSize: 34, fontWeight: 800, marginTop: 10, lineHeight: 1 }}>{value}</div>
            <div className="label-eyebrow" style={{ marginTop: 8 }}>{label}</div>
          </div>
        ))}
      </div>

      {/* AI ideas */}
      <section className="glass glass-hover" style={{ padding: 24 }}>
        <div style={{ display: "flex", flexWrap: "wrap", gap: 12, alignItems: "center", justifyContent: "space-between", marginBottom: 6 }}>
          <div style={{ display: "flex", alignItems: "center", gap: 10 }}>
            <Wand2 size={18} className="ic" />
            <h2 style={{ margin: 0, fontSize: 17, fontWeight: 700 }}>Idées suggérées par l'IA</h2>
          </div>
          <button className="btn btn-ghost" onClick={genIdeas} disabled={loadingIdeas}>
            {loadingIdeas ? <Loader2 size={16} className="spin" /> : <Sparkles size={16} className="ic" />}
            {loadingIdeas ? "Réflexion…" : "Générer des idées"}
          </button>
        </div>
        <p className="muted" style={{ margin: "0 0 16px", fontSize: 13.5 }}>Basées sur ta thématique, tes notes et tes vidéos déjà publiées.</p>

        {err && <div style={{ color: "#e7a", fontSize: 13.5, marginBottom: 12 }}>{err}</div>}
        {!loadingIdeas && suggestions.length === 0 && !err && (
          <div className="muted" style={{ fontSize: 13.5 }}>Renseigne ta thématique dans les réglages et ajoute quelques vidéos pour des suggestions plus pertinentes.</div>
        )}

        <div className="grid-cards" style={{ gridTemplateColumns: "repeat(auto-fit, minmax(260px, 1fr))" }}>
          {suggestions.map((s, i) => (
            <div key={i} className="glass glass-hover fade-in" style={{ padding: 18 }}>
              <div style={{ fontWeight: 700, fontSize: 15, lineHeight: 1.35 }}>{s.title}</div>
              {s.hook && <div style={{ fontSize: 13, marginTop: 10, fontStyle: "italic", color: "#dcdcdc" }}>“{s.hook}”</div>}
              {s.angle && <div className="muted" style={{ fontSize: 12.5, marginTop: 8 }}>{s.angle}</div>}
              {s.why && <div className="muted" style={{ fontSize: 12, marginTop: 8, display: "flex", gap: 6 }}><TrendingUp size={13} /> {s.why}</div>}
              <button className="btn btn-ghost" style={{ marginTop: 14, width: "100%" }} onClick={() => adoptIdea(s)}><Plus size={15} className="ic" /> Ajouter</button>
            </div>
          ))}
        </div>
      </section>
    </div>
  );
}

/* ------------------------------------------------------------------ */
/*  Ideas                                                              */
/* ------------------------------------------------------------------ */
function Ideas({ data, update, notify, openStudioWith }) {
  const [q, setQ] = useState("");
  const [filter, setFilter] = useState("toutes");
  const [editing, setEditing] = useState(null); // idea object or "new"

  const filtered = data.ideas.filter((i) => {
    const okF = filter === "toutes" || i.status === filter;
    const okQ = !q || (i.title + " " + i.notes + " " + i.tags.join(" ")).toLowerCase().includes(q.toLowerCase());
    return okF && okQ;
  });

  const save = (idea) => {
    if (data.ideas.some((i) => i.id === idea.id)) update({ ideas: data.ideas.map((i) => (i.id === idea.id ? idea : i)) });
    else update({ ideas: [idea, ...data.ideas] });
    setEditing(null);
    notify("Idée enregistrée");
  };
  const remove = (id) => { update({ ideas: data.ideas.filter((i) => i.id !== id) }); notify("Idée supprimée"); };
  const setStatus = (id, status) => update({ ideas: data.ideas.map((i) => (i.id === id ? { ...i, status } : i)) });

  return (
    <div className="grid-cards" style={{ gridTemplateColumns: "1fr" }}>
      <section className="glass" style={{ padding: 18, display: "flex", flexWrap: "wrap", gap: 12, alignItems: "center" }}>
        <div style={{ position: "relative", flex: "1 1 220px" }}>
          <Search size={15} style={{ position: "absolute", left: 14, top: 14, color: "#777" }} />
          <input className="field" style={{ paddingLeft: 38 }} placeholder="Rechercher une idée…" value={q} onChange={(e) => setQ(e.target.value)} />
        </div>
        <select className="field" style={{ flex: "0 0 170px" }} value={filter} onChange={(e) => setFilter(e.target.value)}>
          <option value="toutes">Tous les statuts</option>
          {STATUSES.map((s) => <option key={s} value={s}>{s}</option>)}
        </select>
        <button className="btn btn-primary" onClick={() => setEditing("new")}><Plus size={16} className="ic" /> Nouvelle idée</button>
      </section>

      {filtered.length === 0 && (
        <div className="glass" style={{ padding: 40, textAlign: "center" }}>
          <Lightbulb size={26} className="muted" style={{ marginBottom: 12 }} />
          <div className="muted">Aucune idée ici. Lance-toi : note la première qui te passe par la tête.</div>
        </div>
      )}

      <div className="grid-cards" style={{ gridTemplateColumns: "repeat(auto-fit, minmax(290px, 1fr))" }}>
        {filtered.map((i) => (
          <div key={i.id} className="glass glass-hover" style={{ padding: 20, display: "flex", flexDirection: "column" }}>
            <div style={{ display: "flex", justifyContent: "space-between", gap: 8 }}>
              <div style={{ fontWeight: 700, fontSize: 15.5, lineHeight: 1.35 }}>{i.title}</div>
              <div style={{ display: "flex", gap: 6 }}>
                <button className="btn-icon" title="Modifier" onClick={() => setEditing(i)}><Pencil size={14} /></button>
                <button className="btn-icon" title="Supprimer" onClick={() => remove(i.id)}><Trash2 size={14} /></button>
              </div>
            </div>
            {i.notes && <div className="muted" style={{ fontSize: 13, marginTop: 10, whiteSpace: "pre-wrap" }}>{i.notes.slice(0, 180)}{i.notes.length > 180 ? "…" : ""}</div>}
            {i.tags.length > 0 && <div style={{ display: "flex", gap: 6, flexWrap: "wrap", marginTop: 12 }}>{i.tags.map((t) => <span key={t} className="tag">{t}</span>)}</div>}
            {i.script && <div className="chip" style={{ marginTop: 12, alignSelf: "flex-start" }}>Script prêt</div>}
            <div style={{ flex: 1 }} />
            <hr className="hr" style={{ margin: "16px 0 14px" }} />
            <div style={{ display: "flex", gap: 10, alignItems: "center" }}>
              <select className="field" style={{ padding: "8px 12px", fontSize: 12.5 }} value={i.status} onChange={(e) => setStatus(i.id, e.target.value)}>
                {STATUSES.map((s) => <option key={s} value={s}>{s}</option>)}
              </select>
              <button className="btn btn-ghost" style={{ padding: "9px 13px", whiteSpace: "nowrap" }} onClick={() => openStudioWith(i.id)}>
                <FileText size={14} className="ic" /> Script <ArrowRight size={13} />
              </button>
            </div>
          </div>
        ))}
      </div>

      {editing && <IdeaModal idea={editing === "new" ? null : editing} defaults={data.settings} onSave={save} onClose={() => setEditing(null)} />}
    </div>
  );
}

function IdeaModal({ idea, defaults, onSave, onClose }) {
  const [title, setTitle] = useState(idea?.title || "");
  const [notes, setNotes] = useState(idea?.notes || "");
  const [tags, setTags] = useState((idea?.tags || []).join(", "));
  const submit = () => {
    if (!title.trim()) return;
    onSave({
      id: idea?.id || uid(),
      title: title.trim(),
      notes: notes.trim(),
      tags: tags.split(",").map((t) => t.trim()).filter(Boolean),
      status: idea?.status || "idée",
      platform: idea?.platform || defaults.defaultPlatform,
      createdAt: idea?.createdAt || Date.now(),
      script: idea?.script || null,
    });
  };
  return (
    <Modal onClose={onClose} title={idea ? "Modifier l'idée" : "Nouvelle idée"}>
      <label className="label-eyebrow">Titre</label>
      <input className="field" style={{ margin: "6px 0 16px" }} value={title} onChange={(e) => setTitle(e.target.value)} placeholder="Le concept en une ligne" autoFocus />
      <label className="label-eyebrow">Notes</label>
      <textarea className="field" rows={5} style={{ margin: "6px 0 16px" }} value={notes} onChange={(e) => setNotes(e.target.value)} placeholder="Angle, références, ce que tu veux dire…" />
      <label className="label-eyebrow">Tags (séparés par des virgules)</label>
      <input className="field" style={{ margin: "6px 0 18px" }} value={tags} onChange={(e) => setTags(e.target.value)} placeholder="tuto, montage, débutant" />
      <div style={{ display: "flex", gap: 10, justifyContent: "flex-end" }}>
        <button className="btn btn-ghost" onClick={onClose}>Annuler</button>
        <button className="btn btn-primary" onClick={submit} disabled={!title.trim()}><Check size={16} className="ic" /> Enregistrer</button>
      </div>
    </Modal>
  );
}

/* ------------------------------------------------------------------ */
/*  Studio (script generation)                                         */
/* ------------------------------------------------------------------ */
function Studio({ data, update, notify, studioIdeaId, setStudioIdeaId }) {
  const [ideaId, setIdeaId] = useState(studioIdeaId || (data.ideas[0]?.id ?? ""));
  const [freeText, setFreeText] = useState("");
  const [platform, setPlatform] = useState(data.settings.defaultPlatform);
  const [tone, setTone] = useState(data.settings.tone);
  const [duration, setDuration] = useState(DURATIONS[1]);
  const [loading, setLoading] = useState(false);
  const [err, setErr] = useState("");
  const [script, setScript] = useState(null);

  useEffect(() => {
    if (studioIdeaId) {
      setIdeaId(studioIdeaId);
      const found = data.ideas.find((i) => i.id === studioIdeaId);
      if (found?.script) setScript(found.script);
      setStudioIdeaId(null);
    }
  }, [studioIdeaId]);

  const idea = data.ideas.find((i) => i.id === ideaId);

  const generate = async () => {
    setErr(""); setLoading(true); setScript(null);
    const subject = idea ? `${idea.title}\n${idea.notes || ""}` : freeText.trim();
    if (!subject) { setErr("Choisis une idée ou écris un sujet."); setLoading(false); return; }
    try {
      const system = "Tu es un scénariste expert en vidéos format court (TikTok, Reels, YouTube Shorts). Tu écris des scripts en français, oraux, percutants, avec un hook qui scotche dans les 3 premières secondes et une structure qui retient l'attention. Tu réponds UNIQUEMENT en JSON valide, sans texte ni balises autour.";
      const user = `${buildContext(data)}\n\nSUJET DE LA VIDÉO :\n${subject}\n\nContraintes : plateforme ${platform}, ton « ${tone} », durée cible ${duration}.\n\nÉcris le script complet. Donne :\n- un hook principal (1 phrase orale très forte)\n- 2 hooks alternatifs\n- le corps du script découpé en 3 à 5 sections (chaque section : un label court, un timing indicatif type "0–5 s", le texte à dire)\n- un call-to-action final\n- une légende de publication courte\n- 4 hashtags pertinents\n- 2 conseils de tournage/montage propres à ce sujet\n\nFormat JSON strict : {"hook":"","hookAlternatives":["",""],"sections":[{"label":"","timing":"","text":""}],"cta":"","caption":"","hashtags":["","","",""],"tips":["",""]}`;
      const txt = await callClaude(system, user);
      const obj = extractJSON(txt);
      setScript(obj);
    } catch (e) {
      setErr("La génération a échoué. Réessaie — si le sujet est très long, raccourcis un peu tes notes.");
    } finally { setLoading(false); }
  };

  const saveToIdea = () => {
    if (!idea || !script) return;
    update({ ideas: data.ideas.map((i) => (i.id === idea.id ? { ...i, script, status: i.status === "idée" || i.status === "à scripter" ? "scriptée" : i.status } : i)) });
    notify("Script enregistré dans l'idée");
  };

  const copyAll = () => {
    if (!script) return;
    const parts = [
      "HOOK : " + script.hook,
      "", ...(script.sections || []).map((s) => `[${s.timing}] ${s.label}\n${s.text}`),
      "", "CTA : " + script.cta,
      "", "Légende : " + script.caption,
      (script.hashtags || []).join(" "),
    ];
    navigator.clipboard?.writeText(parts.join("\n")).then(() => notify("Script copié"));
  };

  return (
    <div className="grid-cards" style={{ gridTemplateColumns: "1fr" }}>
      <section className="glass glass-hover" style={{ padding: 24 }}>
        <div style={{ display: "flex", alignItems: "center", gap: 10, marginBottom: 16 }}>
          <FileText size={18} className="ic" />
          <h2 style={{ margin: 0, fontSize: 17, fontWeight: 700 }}>Générer un script</h2>
        </div>

        <label className="label-eyebrow">Idée de base</label>
        <select className="field" style={{ margin: "6px 0 14px" }} value={ideaId} onChange={(e) => { setIdeaId(e.target.value); setScript(null); }}>
          <option value="">— Écrire un sujet libre —</option>
          {data.ideas.map((i) => <option key={i.id} value={i.id}>{i.title}</option>)}
        </select>

        {!ideaId && (
          <textarea className="field" rows={3} style={{ marginBottom: 14 }} placeholder="Décris le sujet de ta vidéo…" value={freeText} onChange={(e) => setFreeText(e.target.value)} />
        )}

        <div className="grid-cards" style={{ gridTemplateColumns: "repeat(auto-fit, minmax(160px, 1fr))", marginBottom: 16 }}>
          <div><label className="label-eyebrow">Plateforme</label><select className="field" style={{ marginTop: 6 }} value={platform} onChange={(e) => setPlatform(e.target.value)}>{PLATFORMS.map((p) => <option key={p}>{p}</option>)}</select></div>
          <div><label className="label-eyebrow">Ton</label><select className="field" style={{ marginTop: 6 }} value={tone} onChange={(e) => setTone(e.target.value)}>{TONES.map((t) => <option key={t}>{t}</option>)}</select></div>
          <div><label className="label-eyebrow">Durée</label><select className="field" style={{ marginTop: 6 }} value={duration} onChange={(e) => setDuration(e.target.value)}>{DURATIONS.map((d) => <option key={d}>{d}</option>)}</select></div>
        </div>

        <button className="btn btn-primary" onClick={generate} disabled={loading}>
          {loading ? <Loader2 size={16} className="spin" /> : <Wand2 size={16} className="ic" />}
          {loading ? "Rédaction en cours…" : "Écrire le script"}
        </button>
        {err && <div style={{ color: "#e7a", fontSize: 13.5, marginTop: 12 }}>{err}</div>}
      </section>

      {script && (
        <section className="glass glass-hover fade-in" style={{ padding: 24 }}>
          <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", flexWrap: "wrap", gap: 10, marginBottom: 16 }}>
            <h2 style={{ margin: 0, fontSize: 17, fontWeight: 700 }}>Ton script</h2>
            <div style={{ display: "flex", gap: 8 }}>
              <button className="btn btn-ghost" onClick={copyAll}><Copy size={15} className="ic" /> Copier</button>
              {idea && <button className="btn btn-primary" onClick={saveToIdea}><Check size={15} className="ic" /> Enregistrer</button>}
            </div>
          </div>

          <Block title="Hook">
            <div style={{ fontSize: 16, fontWeight: 600 }}>“{script.hook}”</div>
            {script.hookAlternatives?.length > 0 && (
              <div style={{ marginTop: 12 }}>
                <div className="label-eyebrow" style={{ marginBottom: 8 }}>Variantes</div>
                {script.hookAlternatives.map((h, k) => <div key={k} className="muted" style={{ fontSize: 13.5, marginBottom: 6 }}>· {h}</div>)}
              </div>
            )}
          </Block>

          <Block title="Déroulé">
            {(script.sections || []).map((s, k) => (
              <div key={k} style={{ marginBottom: 16 }}>
                <div style={{ display: "flex", gap: 10, alignItems: "center", marginBottom: 6 }}>
                  <span className="chip"><Clock size={12} style={{ marginRight: 5, verticalAlign: "-2px" }} />{s.timing}</span>
                  <span style={{ fontWeight: 700, fontSize: 13.5 }}>{s.label}</span>
                </div>
                <div style={{ fontSize: 14, lineHeight: 1.6, color: "#e3e3e3" }}>{s.text}</div>
              </div>
            ))}
          </Block>

          <Block title="Call-to-action"><div style={{ fontSize: 14.5, lineHeight: 1.6 }}>{script.cta}</div></Block>
          <Block title="Légende"><div style={{ fontSize: 14, lineHeight: 1.6, color: "#e3e3e3" }}>{script.caption}</div>
            {script.hashtags?.length > 0 && <div style={{ display: "flex", gap: 6, flexWrap: "wrap", marginTop: 10 }}>{script.hashtags.map((h, k) => <span key={k} className="tag"><Hash size={11} style={{ verticalAlign: "-1px" }} /> {h.replace(/^#/, "")}</span>)}</div>}
          </Block>
          {script.tips?.length > 0 && (
            <Block title="Conseils tournage / montage">
              {script.tips.map((t, k) => <div key={k} style={{ fontSize: 13.5, lineHeight: 1.55, marginBottom: 6, display: "flex", gap: 8 }}><Sparkles size={14} className="muted" style={{ flexShrink: 0, marginTop: 3 }} /> {t}</div>)}
            </Block>
          )}
        </section>
      )}
    </div>
  );
}

function Block({ title, children }) {
  return (
    <div style={{ marginBottom: 20 }}>
      <div className="label-eyebrow" style={{ marginBottom: 10 }}>{title}</div>
      <div className="glass" style={{ padding: 16, background: "rgba(255,255,255,0.025)" }}>{children}</div>
    </div>
  );
}

/* ------------------------------------------------------------------ */
/*  Library                                                            */
/* ------------------------------------------------------------------ */
function Library({ data, update, notify }) {
  const [editing, setEditing] = useState(null);

  const save = (v) => {
    if (data.videos.some((x) => x.id === v.id)) update({ videos: data.videos.map((x) => (x.id === v.id ? v : x)) });
    else update({ videos: [v, ...data.videos] });
    setEditing(null);
    notify("Vidéo enregistrée");
  };
  const remove = (id) => { update({ videos: data.videos.filter((v) => v.id !== id) }); notify("Vidéo supprimée"); };

  return (
    <div className="grid-cards" style={{ gridTemplateColumns: "1fr" }}>
      <section className="glass" style={{ padding: 20, display: "flex", justifyContent: "space-between", alignItems: "center", flexWrap: "wrap", gap: 12 }}>
        <div>
          <h2 style={{ margin: 0, fontSize: 17, fontWeight: 700 }}>Bibliothèque de vidéos</h2>
          <p className="muted" style={{ margin: "6px 0 0", fontSize: 13.5 }}>Plus tu renseignes ce qui a marché, plus l'IA vise juste.</p>
        </div>
        <button className="btn btn-primary" onClick={() => setEditing("new")}><Plus size={16} className="ic" /> Ajouter une vidéo</button>
      </section>

      {data.videos.length === 0 && (
        <div className="glass" style={{ padding: 40, textAlign: "center" }}>
          <Film size={26} className="muted" style={{ marginBottom: 12 }} />
          <div className="muted">Aucune vidéo enregistrée. Ajoute tes publications passées pour nourrir les suggestions.</div>
        </div>
      )}

      <div className="grid-cards" style={{ gridTemplateColumns: "repeat(auto-fit, minmax(290px, 1fr))" }}>
        {data.videos.map((v) => (
          <div key={v.id} className="glass glass-hover" style={{ padding: 20 }}>
            <div style={{ display: "flex", justifyContent: "space-between", gap: 8 }}>
              <div style={{ fontWeight: 700, fontSize: 15.5, lineHeight: 1.35 }}>{v.title}</div>
              <div style={{ display: "flex", gap: 6 }}>
                <button className="btn-icon" onClick={() => setEditing(v)}><Pencil size={14} /></button>
                <button className="btn-icon" onClick={() => remove(v.id)}><Trash2 size={14} /></button>
              </div>
            </div>
            <div style={{ display: "flex", gap: 6, flexWrap: "wrap", marginTop: 12 }}>
              {v.platform && <span className="tag">{v.platform}</span>}
              {v.theme && <span className="tag">{v.theme}</span>}
              {v.performance && <span className="chip" style={{ alignSelf: "center" }}><TrendingUp size={11} style={{ verticalAlign: "-1px", marginRight: 4 }} />{v.performance}</span>}
            </div>
            {v.hook && <div style={{ fontSize: 13, marginTop: 12, fontStyle: "italic", color: "#dcdcdc" }}>Hook : “{v.hook}”</div>}
            {v.worked && <div className="muted" style={{ fontSize: 12.5, marginTop: 8 }}>Ce qui a marché : {v.worked}</div>}
          </div>
        ))}
      </div>

      {editing && <VideoModal video={editing === "new" ? null : editing} defaults={data.settings} onSave={save} onClose={() => setEditing(null)} />}
    </div>
  );
}

function VideoModal({ video, defaults, onSave, onClose }) {
  const [f, setF] = useState({
    title: video?.title || "", theme: video?.theme || "", platform: video?.platform || defaults.defaultPlatform,
    hook: video?.hook || "", performance: video?.performance || "", worked: video?.worked || "",
  });
  const set = (k, val) => setF((p) => ({ ...p, [k]: val }));
  const submit = () => { if (!f.title.trim()) return; onSave({ id: video?.id || uid(), createdAt: video?.createdAt || Date.now(), ...f, title: f.title.trim() }); };
  return (
    <Modal onClose={onClose} title={video ? "Modifier la vidéo" : "Ajouter une vidéo"}>
      <label className="label-eyebrow">Titre</label>
      <input className="field" style={{ margin: "6px 0 14px" }} value={f.title} onChange={(e) => set("title", e.target.value)} autoFocus />
      <div className="grid-cards" style={{ gridTemplateColumns: "1fr 1fr", marginBottom: 14 }}>
        <div><label className="label-eyebrow">Thème</label><input className="field" style={{ marginTop: 6 }} value={f.theme} onChange={(e) => set("theme", e.target.value)} placeholder="montage, mindset…" /></div>
        <div><label className="label-eyebrow">Plateforme</label><select className="field" style={{ marginTop: 6 }} value={f.platform} onChange={(e) => set("platform", e.target.value)}>{PLATFORMS.map((p) => <option key={p}>{p}</option>)}</select></div>
      </div>
      <label className="label-eyebrow">Hook utilisé</label>
      <input className="field" style={{ margin: "6px 0 14px" }} value={f.hook} onChange={(e) => set("hook", e.target.value)} />
      <label className="label-eyebrow">Performance (vues / engagement)</label>
      <input className="field" style={{ margin: "6px 0 14px" }} value={f.performance} onChange={(e) => set("performance", e.target.value)} placeholder="ex : 120k vues, fort taux de complétion" />
      <label className="label-eyebrow">Ce qui a marché (ou pas)</label>
      <textarea className="field" rows={3} style={{ margin: "6px 0 18px" }} value={f.worked} onChange={(e) => set("worked", e.target.value)} />
      <div style={{ display: "flex", gap: 10, justifyContent: "flex-end" }}>
        <button className="btn btn-ghost" onClick={onClose}>Annuler</button>
        <button className="btn btn-primary" onClick={submit} disabled={!f.title.trim()}><Check size={16} className="ic" /> Enregistrer</button>
      </div>
    </Modal>
  );
}

/* ------------------------------------------------------------------ */
/*  Settings                                                           */
/* ------------------------------------------------------------------ */
function SettingsView({ data, update, notify }) {
  const [s, setS] = useState(data.settings);
  const set = (k, v) => setS((p) => ({ ...p, [k]: v }));
  const save = () => { update({ settings: s }); notify("Réglages enregistrés"); };
  return (
    <section className="glass glass-hover" style={{ padding: 26, maxWidth: 640 }}>
      <div style={{ display: "flex", alignItems: "center", gap: 10, marginBottom: 6 }}>
        <SettingsIcon size={18} className="ic" />
        <h2 style={{ margin: 0, fontSize: 17, fontWeight: 700 }}>Réglages du studio</h2>
      </div>
      <p className="muted" style={{ margin: "0 0 20px", fontSize: 13.5 }}>Ce profil guide chaque génération d'idée et de script.</p>

      <label className="label-eyebrow">Thématique de la chaîne</label>
      <input className="field" style={{ margin: "6px 0 16px" }} value={s.niche} onChange={(e) => set("niche", e.target.value)} placeholder="ex : montage vidéo pour créateurs débutants" />

      <label className="label-eyebrow">Audience visée</label>
      <input className="field" style={{ margin: "6px 0 16px" }} value={s.audience} onChange={(e) => set("audience", e.target.value)} placeholder="ex : 18–30 ans, débute sur YouTube" />

      <div className="grid-cards" style={{ gridTemplateColumns: "1fr 1fr", marginBottom: 16 }}>
        <div><label className="label-eyebrow">Ton par défaut</label><select className="field" style={{ marginTop: 6 }} value={s.tone} onChange={(e) => set("tone", e.target.value)}>{TONES.map((t) => <option key={t}>{t}</option>)}</select></div>
        <div><label className="label-eyebrow">Plateforme par défaut</label><select className="field" style={{ marginTop: 6 }} value={s.defaultPlatform} onChange={(e) => set("defaultPlatform", e.target.value)}>{PLATFORMS.map((p) => <option key={p}>{p}</option>)}</select></div>
      </div>

      <label className="label-eyebrow">Idées générées par fournée : {s.ideaCount}</label>
      <input type="range" min={3} max={8} value={s.ideaCount} onChange={(e) => set("ideaCount", +e.target.value)} style={{ width: "100%", margin: "12px 0 22px", accentColor: "#fff" }} />

      <button className="btn btn-primary" onClick={save}><Check size={16} className="ic" /> Enregistrer les réglages</button>
    </section>
  );
}

/* ------------------------------------------------------------------ */
/*  Modal shell                                                        */
/* ------------------------------------------------------------------ */
function Modal({ title, children, onClose }) {
  useEffect(() => {
    const h = (e) => e.key === "Escape" && onClose();
    window.addEventListener("keydown", h);
    return () => window.removeEventListener("keydown", h);
  }, [onClose]);
  return (
    <div onClick={onClose} style={{ position: "fixed", inset: 0, background: "rgba(0,0,0,0.6)", backdropFilter: "blur(4px)", zIndex: 60, display: "flex", alignItems: "flex-start", justifyContent: "center", padding: "60px 16px", overflowY: "auto" }}>
      <div onClick={(e) => e.stopPropagation()} className="glass fade-in" style={{ width: "100%", maxWidth: 480, padding: 26 }}>
        <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: 20 }}>
          <h3 style={{ margin: 0, fontSize: 17, fontWeight: 700 }}>{title}</h3>
          <button className="btn-icon" onClick={onClose}><X size={16} /></button>
        </div>
        {children}
      </div>
    </div>
  );
}
