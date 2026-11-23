```aura width=800 height=300
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#07070d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.28)' }}>
  <style>{`
    @keyframes h-orb-1 { 0%, 100% { transform: translate(0, 0); opacity: 0.65; } 50% { transform: translate(34px, -20px); opacity: 0.95; } }
    @keyframes h-orb-2 { 0%, 100% { transform: translate(0, 0); opacity: 0.55; } 50% { transform: translate(-28px, 18px); opacity: 0.85; } }
    @keyframes h-orb-3 { 0%, 100% { transform: translate(0, 0); opacity: 0.45; } 50% { transform: translate(20px, -26px); opacity: 0.75; } }
    @keyframes h-ring { 0%, 100% { opacity: 0.06; } 50% { opacity: 0.19; } }
    @keyframes h-wave { 0% { stroke-dashoffset: 900; } 100% { stroke-dashoffset: 0; } }
    @keyframes h-spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
    #h-o1 { animation: h-orb-1 8.5s ease-in-out infinite; }
    #h-o2 { animation: h-orb-2 10.5s ease-in-out infinite 0.6s; }
    #h-o3 { animation: h-orb-3 9.5s ease-in-out infinite 1.4s; }
    #h-o4 { animation: h-orb-2 11.5s ease-in-out infinite 2.2s; }
    #h-r1 { animation: h-ring 7s ease-in-out infinite; }
    #h-r2 { animation: h-ring 7s ease-in-out infinite 1.8s; }
    #h-r3 { animation: h-ring 9s ease-in-out infinite 3.2s; }
    #h-orbit { transform-origin: 400px 145px; animation: h-spin 18s linear infinite; }
    #h-spark { stroke-dasharray: 900; animation: h-wave 5s linear infinite; }
  `}</style>

  <svg width="800" height="300" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="hg-violet" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.62)" />
        <stop offset="70%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
      <radialGradient id="hg-cyan" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(34,211,238,0.52)" />
        <stop offset="70%" stopColor="rgba(34,211,238,0)" />
      </radialGradient>
      <radialGradient id="hg-indigo" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(79,70,229,0.5)" />
        <stop offset="70%" stopColor="rgba(79,70,229,0)" />
      </radialGradient>
      <radialGradient id="hg-magenta" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(217,70,239,0.38)" />
        <stop offset="70%" stopColor="rgba(217,70,239,0)" />
      </radialGradient>
      <linearGradient id="hg-line" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stopColor="rgba(139,92,246,0)" />
        <stop offset="35%" stopColor="rgba(139,92,246,0.65)" />
        <stop offset="65%" stopColor="rgba(34,211,238,0.75)" />
        <stop offset="100%" stopColor="rgba(34,211,238,0)" />
      </linearGradient>
    </defs>

    <ellipse id="h-o1" cx="140" cy="250" rx="250" ry="170" fill="url(#hg-violet)" />
    <ellipse id="h-o2" cx="680" cy="60" rx="240" ry="165" fill="url(#hg-cyan)" />
    <ellipse id="h-o3" cx="610" cy="275" rx="210" ry="145" fill="url(#hg-indigo)" />
    <ellipse id="h-o4" cx="195" cy="40" rx="185" ry="130" fill="url(#hg-magenta)" />

    <circle id="h-r1" cx="400" cy="145" r="78" fill="none" stroke="rgba(196,181,253,0.9)" strokeWidth="0.7" />
    <circle id="h-r2" cx="400" cy="145" r="132" fill="none" stroke="rgba(165,243,252,0.85)" strokeWidth="0.7" />
    <circle id="h-r3" cx="400" cy="145" r="196" fill="none" stroke="rgba(196,181,253,0.75)" strokeWidth="0.6" />
    <g id="h-orbit">
      <circle cx="400" cy="13" r="3" fill="#22d3ee" />
    </g>

    <path id="h-spark" d="M 0 268 Q 95 258, 165 264 T 320 250 T 485 260 T 640 244 T 800 256" fill="none" stroke="url(#hg-line)" strokeWidth="1.6" />
  </svg>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center' }}>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8, padding: '5px 16px 5px 12px', background: 'rgba(15,23,42,0.62)', borderRadius: 100, border: '1px solid rgba(148,163,184,0.22)', marginBottom: 18 }}>
      <div style={{ width: 8, height: 8, borderRadius: 4, background: '#22c55e', boxShadow: '0 0 8px rgba(34,197,94,0.9)' }} />
      <span style={{ fontSize: 12, color: '#cbd5e1', letterSpacing: 1.2 }}>Cairo, Egypt</span>
    </div>

    <span style={{ fontSize: 48, fontWeight: 700, color: '#ffffff', letterSpacing: -1.5, lineHeight: 1.05 }}>Hi, I'm Mostafa Osama</span>

    <span style={{ fontSize: 16, fontWeight: 600, color: '#67e8f9', marginTop: 12, letterSpacing: 5, textTransform: 'uppercase' }}>Data Analyst</span>

    <div style={{ display: 'flex', gap: 10, marginTop: 22 }}>
      <span style={{ padding: '6px 16px', background: 'rgba(17,15,31,0.68)', color: '#c4b5fd', borderRadius: 100, fontSize: 12, fontWeight: 500, border: '1px solid rgba(139,92,246,0.32)' }}>Power BI</span>
      <span style={{ padding: '6px 16px', background: 'rgba(17,15,31,0.68)', color: '#67e8f9', borderRadius: 100, fontSize: 12, fontWeight: 500, border: '1px solid rgba(34,211,238,0.3)' }}>SQL</span>
      <span style={{ padding: '6px 16px', background: 'rgba(17,15,31,0.68)', color: '#a5b4fc', borderRadius: 100, fontSize: 12, fontWeight: 500, border: '1px solid rgba(129,140,248,0.3)' }}>Python</span>
      <span style={{ padding: '6px 16px', background: 'rgba(17,15,31,0.68)', color: '#86efac', borderRadius: 100, fontSize: 12, fontWeight: 500, border: '1px solid rgba(74,222,128,0.28)' }}>Advanced Excel</span>
      <span style={{ padding: '6px 16px', background: 'rgba(17,15,31,0.68)', color: '#f0abfc', borderRadius: 100, fontSize: 12, fontWeight: 500, border: '1px solid rgba(217,70,239,0.28)' }}>Power Query</span>
    </div>
  </div>
</div>
```

```aura width=176 height=46 link="https://www.linkedin.com/in/mostafaosama0/" inline align=center
<div style={{ position: 'relative', display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', padding: '0 6px', fontFamily: 'Inter, sans-serif' }}>
  <svg width="176" height="46" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <linearGradient id="btn-li-grad" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stopColor="#38bdf8" />
        <stop offset="50%" stopColor="#8b5cf6" />
        <stop offset="100%" stopColor="#22d3ee" />
        <animateTransform attributeName="gradientTransform" type="rotate" from="0 0.5 0.5" to="360 0.5 0.5" dur="4.5s" repeatCount="indefinite" />
      </linearGradient>
    </defs>
    <rect x="7" y="1" width="162" height="44" rx="13" fill="rgba(14,22,38,0.94)" stroke="url(#btn-li-grad)" strokeWidth="1.6" />
    <g transform="translate(32, 13) scale(0.84)">
      <path fill="#38bdf8" d="M19 3a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h14m-.5 15.5v-5.3a3.26 3.26 0 0 0-3.26-3.26c-.85 0-1.84.52-2.28 1.3v-1.11h-2.79v8.37h2.79v-4.93c0-.77.62-1.4 1.39-1.4a1.4 1.4 0 0 1 1.4 1.4v4.93h2.75M6.88 8.56a1.68 1.68 0 0 0 1.68-1.68c0-.93-.75-1.69-1.68-1.69a1.69 1.69 0 0 0-1.69 1.69c0 .93.76 1.68 1.69 1.68m1.39 9.94v-8.37H5.5v8.37h2.77z" />
    </g>
  </svg>
  <span style={{ fontSize: 13.5, fontWeight: 600, color: '#f8fafc', marginLeft: 24, letterSpacing: 0.3 }}>LinkedIn</span>
</div>
```

```aura width=166 height=46 link="mailto:mostafaosama7213@gmail.com" inline align=center
<div style={{ position: 'relative', display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', padding: '0 6px', fontFamily: 'Inter, sans-serif' }}>
  <svg width="166" height="46" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <linearGradient id="btn-em-grad" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stopColor="#f472b6" />
        <stop offset="50%" stopColor="#8b5cf6" />
        <stop offset="100%" stopColor="#fb7185" />
        <animateTransform attributeName="gradientTransform" type="rotate" from="0 0.5 0.5" to="360 0.5 0.5" dur="4.5s" repeatCount="indefinite" />
      </linearGradient>
    </defs>
    <rect x="7" y="1" width="152" height="44" rx="13" fill="rgba(26,12,28,0.94)" stroke="url(#btn-em-grad)" strokeWidth="1.6" />
    <g transform="translate(36, 13) scale(0.84)">
      <path fill="#fb7185" d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4-8 5-8-5V6l8 5 8-5v2z" />
    </g>
  </svg>
  <span style={{ fontSize: 13.5, fontWeight: 600, color: '#f8fafc', marginLeft: 24, letterSpacing: 0.3 }}>Email</span>
</div>
```

```aura width=166 height=46 link="https://github.com/MostafaOsama0" inline align=center
<div style={{ position: 'relative', display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', padding: '0 6px', fontFamily: 'Inter, sans-serif' }}>
  <svg width="166" height="46" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <linearGradient id="btn-gh-grad" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stopColor="#c4b5fd" />
        <stop offset="50%" stopColor="#22d3ee" />
        <stop offset="100%" stopColor="#818cf8" />
        <animateTransform attributeName="gradientTransform" type="rotate" from="0 0.5 0.5" to="360 0.5 0.5" dur="4.5s" repeatCount="indefinite" />
      </linearGradient>
    </defs>
    <rect x="7" y="1" width="152" height="44" rx="13" fill="rgba(16,14,28,0.94)" stroke="url(#btn-gh-grad)" strokeWidth="1.6" />
    <g transform="translate(33, 13) scale(0.84)">
      <path fill="#e2e8f0" d="M12 2A10 10 0 0 0 2 12c0 4.42 2.87 8.17 6.84 9.5.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34-.46-1.16-1.11-1.47-1.11-1.47-.91-.62.07-.6.07-.6 1 .07 1.53 1.03 1.53 1.03.87 1.52 2.34 1.07 2.91.83.09-.65.35-1.09.63-1.34-2.22-.25-4.55-1.11-4.55-4.92 0-1.11.38-2 1.03-2.71-.1-.25-.45-1.29.1-2.64 0 0 .84-.27 2.75 1.02.79-.22 1.65-.33 2.5-.33.85 0 1.71.11 2.5.33 1.91-1.29 2.75-1.02 2.75-1.02.55 1.35.2 2.39.1 2.64.65.71 1.03 1.6 1.03 2.71 0 3.82-2.34 4.66-4.57 4.91.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2z" />
    </g>
  </svg>
  <span style={{ fontSize: 13.5, fontWeight: 600, color: '#f8fafc', marginLeft: 24, letterSpacing: 0.3 }}>GitHub</span>
</div>
```

```aura width=800 height=250
<div style={{ position: 'relative', display: 'flex', flexDirection: 'row', width: '100%', height: '100%', background: '#07070d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.24)', padding: 24, gap: 18 }}>
  <style>{`
    @keyframes ab-drift-1 { 0%, 100% { transform: translate(0, 0); opacity: 0.55; } 50% { transform: translate(24px, -14px); opacity: 0.85; } }
    @keyframes ab-drift-2 { 0%, 100% { transform: translate(0, 0); opacity: 0.45; } 50% { transform: translate(-20px, 14px); opacity: 0.78; } }
    @keyframes ab-shimmer { 0% { transform: translateX(-120px); opacity: 0; } 50% { opacity: 0.45; } 100% { transform: translateX(260px); opacity: 0; } }
    #ab-g1 { animation: ab-drift-1 8s ease-in-out infinite; }
    #ab-g2 { animation: ab-drift-2 10s ease-in-out infinite 0.8s; }
    #ab-beam { animation: ab-shimmer 4.2s ease-in-out infinite; }
  `}</style>

  <svg width="800" height="250" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ab-rg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.48)" />
        <stop offset="70%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
      <radialGradient id="ab-rg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(34,211,238,0.42)" />
        <stop offset="70%" stopColor="rgba(34,211,238,0)" />
      </radialGradient>
      <linearGradient id="ab-shine" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stopColor="rgba(34,211,238,0)" />
        <stop offset="50%" stopColor="rgba(196,181,253,0.28)" />
        <stop offset="100%" stopColor="rgba(34,211,238,0)" />
      </linearGradient>
    </defs>
    <ellipse id="ab-g1" cx="120" cy="215" rx="220" ry="135" fill="url(#ab-rg1)" />
    <ellipse id="ab-g2" cx="710" cy="45" rx="215" ry="135" fill="url(#ab-rg2)" />
    <rect id="ab-beam" x="550" y="24" width="90" height="202" fill="url(#ab-shine)" />
  </svg>

  <div style={{ display: 'flex', flexDirection: 'column', flex: 1, justifyContent: 'center', background: 'rgba(15,14,28,0.62)', borderRadius: 16, padding: '18px 22px', border: '1px solid rgba(148,163,184,0.16)' }}>
    <span style={{ fontSize: 11, fontWeight: 700, color: '#67e8f9', letterSpacing: 2.5, textTransform: 'uppercase', marginBottom: 10 }}>About Me · Data Analyst</span>
    <span style={{ fontSize: 12.6, color: '#e2e8f0', lineHeight: 1.54 }}>
      Data Analyst skilled in Power BI, SQL, Python, and Excel, with experience building end-to-end analytics projects that transform raw data into actionable business insights. Developed interactive dashboards, automated data preparation workflows, and performance analyses across sales, HR, marketing, and operational datasets. Experienced in data cleaning, ETL, data modeling, KPI development, and data visualization, with a focus on delivering clear, data-driven recommendations that support decision-making.
    </span>
  </div>

  <div style={{ display: 'flex', flexDirection: 'column', width: 222, flexShrink: 0, justifyContent: 'center', gap: 11, background: 'rgba(15,14,28,0.62)', borderRadius: 16, padding: '16px 18px', border: '1px solid rgba(139,92,246,0.24)' }}>
    <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 2 }}>
      <span style={{ fontSize: 10.5, fontWeight: 700, color: '#a5b4fc', letterSpacing: 2, textTransform: 'uppercase' }}>Top Languages</span>
      <span style={{ fontSize: 9.5, color: '#67e8f9', letterSpacing: 1 }}>LIVE</span>
    </div>
    {(github && github.languages && github.languages.length > 0
      ? github.languages.slice(0, 4)
      : [
          { name: 'SQL', percentage: 40, color: '#22d3ee' },
          { name: 'Python', percentage: 35, color: '#a78bfa' },
          { name: 'Power BI', percentage: 15, color: '#818cf8' },
          { name: 'Excel', percentage: 10, color: '#86efac' },
        ]
    ).map((lang, idx) => (
      <div key={idx} style={{ display: 'flex', flexDirection: 'column', gap: 4 }}>
        <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between' }}>
          <div style={{ display: 'flex', alignItems: 'center', gap: 6 }}>
            <div style={{ width: 7, height: 7, borderRadius: 4, background: lang.color || '#22d3ee' }} />
            <span style={{ fontSize: 11.5, fontWeight: 600, color: '#f1f5f9' }}>{lang.name}</span>
          </div>
          <span style={{ fontSize: 11, fontWeight: 600, color: '#94a3b8' }}>{lang.percentage}%</span>
        </div>
        <div style={{ display: 'flex', width: '100%', height: 6, background: 'rgba(255,255,255,0.07)', borderRadius: 100, overflow: 'hidden' }}>
          <div style={{ width: `${Math.max(lang.percentage, 8)}%`, height: '100%', background: lang.color || '#8b5cf6', borderRadius: 100 }} />
        </div>
      </div>
    ))}
  </div>
</div>
```

```aura width=800 height=120
<div style={{ position: 'relative', display: 'flex', flexDirection: 'row', alignItems: 'center', justifyContent: 'space-between', gap: 14, width: '100%', height: '100%', background: '#07070d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.22)', padding: '18px 22px' }}>
  <style>{`
    @keyframes st-drift { 0%, 100% { transform: translate(0, 0); opacity: 0.45; } 50% { transform: translate(26px, -10px); opacity: 0.8; } }
    #st-glow1 { animation: st-drift 9s ease-in-out infinite; }
    #st-glow2 { animation: st-drift 11s ease-in-out infinite reverse; }
  `}</style>

  <svg width="800" height="120" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="st-rg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.48)" />
        <stop offset="70%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
      <radialGradient id="st-rg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(34,211,238,0.42)" />
        <stop offset="70%" stopColor="rgba(34,211,238,0)" />
      </radialGradient>
    </defs>
    <ellipse id="st-glow1" cx="180" cy="60" rx="190" ry="90" fill="url(#st-rg1)" />
    <ellipse id="st-glow2" cx="630" cy="60" rx="190" ry="90" fill="url(#st-rg2)" />
  </svg>

  {[
    { label: 'PUBLIC REPOS', value: String(github?.stats?.totalRepos ?? 12), accent: '#a78bfa' },
    { label: 'TOTAL STARS', value: String(github?.stats?.totalStars ?? 0), accent: '#22d3ee' },
    { label: 'TOTAL COMMITS', value: String(github?.stats?.totalCommits ?? 0), accent: '#818cf8' },
    { label: 'TOTAL FORKS', value: String(github?.stats?.totalForks ?? 0), accent: '#f0abfc' },
  ].map((stat, idx) => (
    <div key={idx} style={{ display: 'flex', flexDirection: 'column', flex: 1, height: '100%', alignItems: 'center', justifyContent: 'center', background: 'rgba(15,14,28,0.65)', borderRadius: 14, border: '1px solid rgba(148,163,184,0.16)', zIndex: 10 }}>
      <span style={{ fontSize: 26, fontWeight: 700, color: stat.accent, lineHeight: 1.1 }}>{stat.value}</span>
      <span style={{ fontSize: 10, fontWeight: 600, color: '#94a3b8', letterSpacing: 1.8, marginTop: 6 }}>{stat.label}</span>
    </div>
  ))}
</div>
```

```aura width=800 height=320
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.24)', padding: '22px 26px' }}>
  <style>{`
    @keyframes sk-o1 { 0%, 100% { transform: translate(0, 0); opacity: 0.5; } 50% { transform: translate(30px, -16px); opacity: 0.85; } }
    @keyframes sk-o2 { 0%, 100% { transform: translate(0, 0); opacity: 0.45; } 50% { transform: translate(-26px, 16px); opacity: 0.8; } }
    #sk-g1 { animation: sk-o1 9s ease-in-out infinite; }
    #sk-g2 { animation: sk-o2 11s ease-in-out infinite 0.7s; }
  `}</style>

  <svg width="800" height="320" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="sk-rg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(139,92,246,0.45)" />
        <stop offset="70%" stopColor="rgba(139,92,246,0)" />
      </radialGradient>
      <radialGradient id="sk-rg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(34,211,238,0.4)" />
        <stop offset="70%" stopColor="rgba(34,211,238,0)" />
      </radialGradient>
    </defs>
    <ellipse id="sk-g1" cx="120" cy="270" rx="230" ry="150" fill="url(#sk-rg1)" />
    <ellipse id="sk-g2" cx="690" cy="50" rx="220" ry="145" fill="url(#sk-rg2)" />
  </svg>

  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 16, zIndex: 10 }}>
    <span style={{ fontSize: 19, fontWeight: 700, color: '#ffffff', letterSpacing: -0.3 }}>Skills</span>
    <span style={{ fontSize: 11, color: '#67e8f9', letterSpacing: 2, textTransform: 'uppercase' }}>Technical & Analytical Toolkit</span>
  </div>

  <div style={{ display: 'flex', flexDirection: 'row', gap: 16, flex: 1, zIndex: 10 }}>
    <div style={{ display: 'flex', flexDirection: 'column', flex: 1.35, gap: 9, background: 'rgba(15,14,28,0.65)', borderRadius: 16, padding: '16px 18px', border: '1px solid rgba(139,92,246,0.2)' }}>
      <span style={{ fontSize: 10.5, fontWeight: 700, color: '#a5b4fc', letterSpacing: 1.8, textTransform: 'uppercase', marginBottom: 2 }}>Technical Stack</span>
      {[
        { name: 'Advanced Excel', detail: 'VLookup, Conditional Formatting, Pivot Tables, Formulas', color: '#86efac' },
        { name: 'Power BI', detail: 'Dashboarding, Data Visualization', color: '#fde047' },
        { name: 'SQL', detail: '', color: '#67e8f9' },
        { name: 'Python', detail: 'Pandas, NumPy, Matpolib', color: '#a5b4fc' },
        { name: 'Power Query', detail: 'ETL, Data Transformation', color: '#f0abfc' },
      ].map((s, idx) => (
        <div key={idx} style={{ display: 'flex', alignItems: 'center', gap: 8, padding: '6px 10px', background: 'rgba(255,255,255,0.03)', borderRadius: 10, border: '1px solid rgba(255,255,255,0.07)' }}>
          <div style={{ width: 6, height: 6, borderRadius: 3, background: s.color, flexShrink: 0 }} />
          <span style={{ fontSize: 12.5, fontWeight: 700, color: '#f8fafc', flexShrink: 0 }}>{s.name}</span>
          {s.detail ? <span style={{ fontSize: 11.5, color: '#94a3b8' }}>({s.detail})</span> : null}
        </div>
      ))}
    </div>

    <div style={{ display: 'flex', flexDirection: 'column', flex: 0.85, gap: 9, background: 'rgba(15,14,28,0.65)', borderRadius: 16, padding: '16px 18px', border: '1px solid rgba(34,211,238,0.2)' }}>
      <span style={{ fontSize: 10.5, fontWeight: 700, color: '#67e8f9', letterSpacing: 1.8, textTransform: 'uppercase', marginBottom: 2 }}>Core Strengths</span>
      {[
        'Data Storytelling',
        'Analytical Thinking',
        'Problem solving',
        'Communication Skills',
        'Team Collaboration',
      ].map((soft, idx) => (
        <div key={idx} style={{ display: 'flex', alignItems: 'center', gap: 9, padding: '7px 12px', background: 'rgba(34,211,238,0.06)', borderRadius: 10, border: '1px solid rgba(34,211,238,0.16)' }}>
          <div style={{ width: 6, height: 6, borderRadius: 3, background: '#22d3ee', flexShrink: 0 }} />
          <span style={{ fontSize: 12.5, fontWeight: 600, color: '#e2e8f0' }}>{soft}</span>
        </div>
      ))}
    </div>
  </div>
</div>
```

```aura width=800 height=76
<div style={{ position: 'relative', display: 'flex', alignItems: 'center', justifyContent: 'space-between', width: '100%', height: '100%', background: '#07070d', borderRadius: 16, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.28)', padding: '0 26px' }}>
  <style>{`
    @keyframes ph-sweep { 0% { transform: translateX(-200px); } 100% { transform: translateX(900px); } }
    #ph-beam { animation: ph-sweep 4.5s linear infinite; }
  `}</style>
  <svg width="800" height="76" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <linearGradient id="ph-g" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stopColor="rgba(139,92,246,0)" />
        <stop offset="50%" stopColor="rgba(34,211,238,0.32)" />
        <stop offset="100%" stopColor="rgba(34,211,238,0)" />
      </linearGradient>
    </defs>
    <rect id="ph-beam" x="0" y="0" width="200" height="76" fill="url(#ph-g)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', gap: 12, zIndex: 10 }}>
    <div style={{ width: 10, height: 10, borderRadius: 5, background: '#22d3ee' }} />
    <span style={{ fontSize: 20, fontWeight: 700, color: '#ffffff', letterSpacing: -0.3 }}>Projects</span>
  </div>
  <span style={{ fontSize: 11.5, color: '#a5b4fc', letterSpacing: 1.5, textTransform: 'uppercase', zIndex: 10 }}>12 End-to-End Analytics Projects · Click any card to view repo</span>
</div>
```

```aura width=800 height=238 link="https://github.com/MostafaOsama0/Olist-ECommerce-Analytics"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 18, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.28)', padding: '20px 26px' }}>
  <style>{`
    @keyframes p1-o { 0%, 100% { transform: translate(0, 0); opacity: 0.45; } 50% { transform: translate(24px, -12px); opacity: 0.78; } }
    #p1-g1 { animation: p1-o 8s ease-in-out infinite; }
    #p1-g2 { animation: p1-o 10s ease-in-out infinite reverse; }
  `}</style>
  <svg width="800" height="238" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="p1-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(139,92,246,0.45)" /><stop offset="70%" stopColor="rgba(139,92,246,0)" /></radialGradient>
      <radialGradient id="p1-rg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.38)" /><stop offset="70%" stopColor="rgba(34,211,238,0)" /></radialGradient>
    </defs>
    <ellipse id="p1-g1" cx="90" cy="210" rx="200" ry="120" fill="url(#p1-rg1)" />
    <ellipse id="p1-g2" cx="720" cy="35" rx="180" ry="110" fill="url(#p1-rg2)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 14, zIndex: 10 }}>
    <span style={{ fontSize: 18, fontWeight: 700, color: '#ffffff' }}>Olist-ECommerce-Analytics</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
      <span style={{ padding: '4px 12px', background: 'rgba(139,92,246,0.18)', color: '#c4b5fd', borderRadius: 100, fontSize: 11, fontWeight: 600, border: '1px solid rgba(139,92,246,0.35)' }}>Aug 2026</span>
      <span style={{ padding: '4px 10px', background: 'rgba(34,211,238,0.12)', color: '#67e8f9', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>View Repo -&gt;</span>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 9, background: 'rgba(15,14,28,0.62)', borderRadius: 14, padding: '14px 18px', border: '1px solid rgba(148,163,184,0.14)', zIndex: 10, flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Engineered an interactive Power BI solution analyzing 100K+ Brazilian e-commerce orders and $16.01M+ in revenue to evaluate sales trends, regional logistics, and customer retention.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#a78bfa', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Implemented complex DAX calculations (CALCULATE, CROSSFILTER, AVERAGEX) to isolate satisfaction drivers and track customer loyalty segments.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Uncovered a 3.12% customer repeat rate and proved the direct impact of shipping delays on customer sentiment, with 1-star reviews taking double the delivery time (~20 days) of 5-star orders (~9 days).</span></div>
  </div>
</div>
```

```aura width=800 height=238 link="https://github.com/MostafaOsama0/HR-Database-Management-SQL"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 18, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(34,211,238,0.28)', padding: '20px 26px' }}>
  <style>{`
    @keyframes p2-o { 0%, 100% { transform: translate(0, 0); opacity: 0.45; } 50% { transform: translate(-24px, 12px); opacity: 0.78; } }
    #p2-g1 { animation: p2-o 9s ease-in-out infinite; }
    #p2-g2 { animation: p2-o 11s ease-in-out infinite reverse; }
  `}</style>
  <svg width="800" height="238" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="p2-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.42)" /><stop offset="70%" stopColor="rgba(34,211,238,0)" /></radialGradient>
      <radialGradient id="p2-rg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(99,102,241,0.42)" /><stop offset="70%" stopColor="rgba(99,102,241,0)" /></radialGradient>
    </defs>
    <ellipse id="p2-g1" cx="110" cy="40" rx="190" ry="110" fill="url(#p2-rg1)" />
    <ellipse id="p2-g2" cx="700" cy="210" rx="200" ry="120" fill="url(#p2-rg2)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 14, zIndex: 10 }}>
    <span style={{ fontSize: 18, fontWeight: 700, color: '#ffffff' }}>HR-Database-Management-SQL</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
      <span style={{ padding: '4px 12px', background: 'rgba(139,92,246,0.18)', color: '#c4b5fd', borderRadius: 100, fontSize: 11, fontWeight: 600, border: '1px solid rgba(139,92,246,0.35)' }}>Aug 2026</span>
      <span style={{ padding: '4px 10px', background: 'rgba(34,211,238,0.12)', color: '#67e8f9', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>View Repo -&gt;</span>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 9, background: 'rgba(15,14,28,0.62)', borderRadius: 14, padding: '14px 18px', border: '1px solid rgba(148,163,184,0.14)', zIndex: 10, flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Designed a 3NF normalized database schema from scratch, establishing primary and foreign key constraints to eliminate data redundancy across core business entities.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#a78bfa', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Authored optimized SQL scripts and views using CTEs, multi-table joins, and window functions (DENSE_RANK, ROW_NUMBER) to solve multi-layered business intelligence questions.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Transformed raw transactional records into clean, aggregation-ready datasets structured for seamless consumption in BI dashboards and reporting tools.</span></div>
  </div>
</div>
```

```aura width=800 height=238 link="https://github.com/MostafaOsama0/UK_Youtubers_ROI_Analysis"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 18, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(217,70,239,0.26)', padding: '20px 26px' }}>
  <style>{`
    @keyframes p3-o { 0%, 100% { transform: translate(0, 0); opacity: 0.42; } 50% { transform: translate(22px, -14px); opacity: 0.76; } }
    #p3-g1 { animation: p3-o 8.5s ease-in-out infinite; }
    #p3-g2 { animation: p3-o 10.5s ease-in-out infinite reverse; }
  `}</style>
  <svg width="800" height="238" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="p3-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(217,70,239,0.4)" /><stop offset="70%" stopColor="rgba(217,70,239,0)" /></radialGradient>
      <radialGradient id="p3-rg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(139,92,246,0.42)" /><stop offset="70%" stopColor="rgba(139,92,246,0)" /></radialGradient>
    </defs>
    <ellipse id="p3-g1" cx="100" cy="210" rx="190" ry="115" fill="url(#p3-rg1)" />
    <ellipse id="p3-g2" cx="710" cy="40" rx="190" ry="115" fill="url(#p3-rg2)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 14, zIndex: 10 }}>
    <span style={{ fontSize: 18, fontWeight: 700, color: '#ffffff' }}>UK_Youtubers_ROI_Analysis</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
      <span style={{ padding: '4px 12px', background: 'rgba(217,70,239,0.16)', color: '#f0abfc', borderRadius: 100, fontSize: 11, fontWeight: 600, border: '1px solid rgba(217,70,239,0.32)' }}>July 2025</span>
      <span style={{ padding: '4px 10px', background: 'rgba(34,211,238,0.12)', color: '#67e8f9', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>View Repo -&gt;</span>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 9, background: 'rgba(15,14,28,0.62)', borderRadius: 14, padding: '14px 18px', border: '1px solid rgba(148,163,184,0.14)', zIndex: 10, flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#f0abfc', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Developed a dynamic Power BI simulation tool for UK influencer marketing, forecasting Net Profit and ROI using interactive "What-If" cost and conversion scenarios.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#a78bfa', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Implemented advanced DAX logic to correctly model portfolio profitability and created a two-page flow linking financial results to granular Audience Quality metrics.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Demonstrated a full BI workflow by integrating SQL data preparation with professional visualization for actionable, data-driven decision support.</span></div>
  </div>
</div>
```

```aura width=800 height=215 link="https://github.com/MostafaOsama0/US_Dataset-Project"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 18, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.24)', padding: '20px 26px' }}>
  <style>{`
    @keyframes p4-o { 0%, 100% { transform: translate(0, 0); opacity: 0.4; } 50% { transform: translate(20px, -12px); opacity: 0.72; } }
    #p4-g1 { animation: p4-o 9.5s ease-in-out infinite; }
  `}</style>
  <svg width="800" height="215" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="p4-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.4)" /><stop offset="70%" stopColor="rgba(34,211,238,0)" /></radialGradient></defs>
    <ellipse id="p4-g1" cx="680" cy="180" rx="210" ry="110" fill="url(#p4-rg1)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 12, zIndex: 10 }}>
    <span style={{ fontSize: 17.5, fontWeight: 700, color: '#ffffff' }}>US Sales Data Analysis</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
      <span style={{ padding: '4px 12px', background: 'rgba(139,92,246,0.16)', color: '#c4b5fd', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>Sep 2024</span>
      <span style={{ padding: '4px 10px', background: 'rgba(34,211,238,0.12)', color: '#67e8f9', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>View Repo -&gt;</span>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 8, background: 'rgba(15,14,28,0.62)', borderRadius: 14, padding: '14px 18px', border: '1px solid rgba(148,163,184,0.14)', zIndex: 10, flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Analyzed job market data for analytics roles using Excel to identify key hiring trends and insights.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#a78bfa', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Developed PivotTables to evaluate performance by ship mode, product sub-category, and overall category.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Designed an interactive dashboard with dynamic charts to visualize key metrics and support data-driven decision-making.</span></div>
  </div>
</div>
```

```aura width=800 height=215 link="https://github.com/MostafaOsama0/Pizza-Store"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 18, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.24)', padding: '20px 26px' }}>
  <style>{`
    @keyframes p5-o { 0%, 100% { transform: translate(0, 0); opacity: 0.4; } 50% { transform: translate(-22px, 12px); opacity: 0.72; } }
    #p5-g1 { animation: p5-o 8.8s ease-in-out infinite; }
  `}</style>
  <svg width="800" height="215" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="p5-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(139,92,246,0.42)" /><stop offset="70%" stopColor="rgba(139,92,246,0)" /></radialGradient></defs>
    <ellipse id="p5-g1" cx="140" cy="40" rx="210" ry="110" fill="url(#p5-rg1)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 12, zIndex: 10 }}>
    <span style={{ fontSize: 17.5, fontWeight: 700, color: '#ffffff' }}>Pizza Store Data Analysis</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
      <span style={{ padding: '4px 12px', background: 'rgba(139,92,246,0.16)', color: '#c4b5fd', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>Oct 2024</span>
      <span style={{ padding: '4px 10px', background: 'rgba(34,211,238,0.12)', color: '#67e8f9', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>View Repo -&gt;</span>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 8, background: 'rgba(15,14,28,0.62)', borderRadius: 14, padding: '14px 18px', border: '1px solid rgba(148,163,184,0.14)', zIndex: 10, flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Performed ETL processes using Power Query to clean, transform, and structure raw data for analysis.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#a78bfa', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Developed key performance indicators (KPIs) to assess and monitor store growth potential.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Visualized insights through interactive Power BI dashboards, enabling data-driven business decisions.</span></div>
  </div>
</div>
```

```aura width=800 height=215 link="https://github.com/MostafaOsama0/Social-media-metrics-Project/tree/main"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 18, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(34,211,238,0.24)', padding: '20px 26px' }}>
  <style>{`
    @keyframes p6-o { 0%, 100% { transform: translate(0, 0); opacity: 0.4; } 50% { transform: translate(22px, -10px); opacity: 0.72; } }
    #p6-g1 { animation: p6-o 9.2s ease-in-out infinite; }
  `}</style>
  <svg width="800" height="215" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="p6-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(79,70,229,0.44)" /><stop offset="70%" stopColor="rgba(79,70,229,0)" /></radialGradient></defs>
    <ellipse id="p6-g1" cx="690" cy="45" rx="205" ry="110" fill="url(#p6-rg1)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 12, zIndex: 10 }}>
    <span style={{ fontSize: 17.5, fontWeight: 700, color: '#ffffff' }}>Social Media Metrics Dashboard</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
      <span style={{ padding: '4px 12px', background: 'rgba(139,92,246,0.16)', color: '#c4b5fd', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>Sep 2024</span>
      <span style={{ padding: '4px 10px', background: 'rgba(34,211,238,0.12)', color: '#67e8f9', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>View Repo -&gt;</span>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 8, background: 'rgba(15,14,28,0.62)', borderRadius: 14, padding: '14px 18px', border: '1px solid rgba(148,163,184,0.14)', zIndex: 10, flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Developed an Excel dashboard to monitor total impressions across multiple social media platforms.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#a78bfa', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Ensured data accuracy and completeness through transformation and validation processes.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Visualized key performance metrics using Excel charts to deliver clear, actionable insights.</span></div>
  </div>
</div>
```

```aura width=800 height=215 link="https://github.com/MostafaOsama0/Sales_Dataset-Project"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 18, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.24)', padding: '20px 26px' }}>
  <style>{`
    @keyframes p7-o { 0%, 100% { transform: translate(0, 0); opacity: 0.4; } 50% { transform: translate(-20px, -12px); opacity: 0.72; } }
    #p7-g1 { animation: p7-o 9s ease-in-out infinite; }
  `}</style>
  <svg width="800" height="215" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="p7-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.4)" /><stop offset="70%" stopColor="rgba(34,211,238,0)" /></radialGradient></defs>
    <ellipse id="p7-g1" cx="120" cy="185" rx="200" ry="105" fill="url(#p7-rg1)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 12, zIndex: 10 }}>
    <span style={{ fontSize: 17.5, fontWeight: 700, color: '#ffffff' }}>Sales Dataset Analysis</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
      <span style={{ padding: '4px 12px', background: 'rgba(139,92,246,0.16)', color: '#c4b5fd', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>Aug 2024</span>
      <span style={{ padding: '4px 10px', background: 'rgba(34,211,238,0.12)', color: '#67e8f9', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>View Repo -&gt;</span>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 8, background: 'rgba(15,14,28,0.62)', borderRadius: 14, padding: '14px 18px', border: '1px solid rgba(148,163,184,0.14)', zIndex: 10, flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Analyzed sales operations across multiple markets using Excel to uncover performance trends and insights.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#a78bfa', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Cleaned and transformed data, performing text analysis to identify market-specific sales patterns.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Developed an interactive dashboard to visualize market performance and support strategic decision-making.</span></div>
  </div>
</div>
```

```aura width=800 height=215 link="https://github.com/MostafaOsama0/Vrinda-store-Analysis"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 18, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(217,70,239,0.22)', padding: '20px 26px' }}>
  <style>{`
    @keyframes p8-o { 0%, 100% { transform: translate(0, 0); opacity: 0.4; } 50% { transform: translate(20px, 12px); opacity: 0.72; } }
    #p8-g1 { animation: p8-o 8.6s ease-in-out infinite; }
  `}</style>
  <svg width="800" height="215" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="p8-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(217,70,239,0.38)" /><stop offset="70%" stopColor="rgba(217,70,239,0)" /></radialGradient></defs>
    <ellipse id="p8-g1" cx="670" cy="180" rx="205" ry="110" fill="url(#p8-rg1)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 12, zIndex: 10 }}>
    <span style={{ fontSize: 17.5, fontWeight: 700, color: '#ffffff' }}>Vrinda Store Analysis</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
      <span style={{ padding: '4px 12px', background: 'rgba(139,92,246,0.16)', color: '#c4b5fd', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>Aug 2024</span>
      <span style={{ padding: '4px 10px', background: 'rgba(34,211,238,0.12)', color: '#67e8f9', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>View Repo -&gt;</span>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 8, background: 'rgba(15,14,28,0.62)', borderRadius: 14, padding: '14px 18px', border: '1px solid rgba(148,163,184,0.14)', zIndex: 10, flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#f0abfc', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Analyzed store data using Excel to improve reporting accuracy and data clarity.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#a78bfa', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Applied advanced Excel functions to clean, transform, and filter datasets for deeper analysis.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Developed visual reports and charts to highlight key business insights and enhance sales performance.</span></div>
  </div>
</div>
```

```aura width=800 height=205 link="https://github.com/MostafaOsama0/HR-Project"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 18, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.24)', padding: '20px 26px' }}>
  <style>{`
    @keyframes p9-o { 0%, 100% { transform: translate(0, 0); opacity: 0.4; } 50% { transform: translate(-22px, 12px); opacity: 0.72; } }
    #p9-g1 { animation: p9-o 9.4s ease-in-out infinite; }
  `}</style>
  <svg width="800" height="205" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="p9-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(139,92,246,0.42)" /><stop offset="70%" stopColor="rgba(139,92,246,0)" /></radialGradient></defs>
    <ellipse id="p9-g1" cx="130" cy="40" rx="200" ry="105" fill="url(#p9-rg1)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 12, zIndex: 10 }}>
    <span style={{ fontSize: 17.5, fontWeight: 700, color: '#ffffff' }}>HR Project</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
      <span style={{ padding: '4px 12px', background: 'rgba(139,92,246,0.16)', color: '#c4b5fd', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>Sep 2024</span>
      <span style={{ padding: '4px 10px', background: 'rgba(34,211,238,0.12)', color: '#67e8f9', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>View Repo -&gt;</span>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 8, background: 'rgba(15,14,28,0.62)', borderRadius: 14, padding: '14px 18px', border: '1px solid rgba(148,163,184,0.14)', zIndex: 10, flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Designed an HR analytics dashboard using Power BI and Power Query.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#a78bfa', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Processed employee data to track salaries, performance, and attrition trends.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Created interactive visualizations for better workforce insights.</span></div>
  </div>
</div>
```

```aura width=800 height=215 link="https://github.com/MostafaOsama0/HR-Analysis"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 18, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(34,211,238,0.24)', padding: '20px 26px' }}>
  <style>{`
    @keyframes p10-o { 0%, 100% { transform: translate(0, 0); opacity: 0.4; } 50% { transform: translate(22px, -12px); opacity: 0.72; } }
    #p10-g1 { animation: p10-o 8.7s ease-in-out infinite; }
  `}</style>
  <svg width="800" height="215" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="p10-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.4)" /><stop offset="70%" stopColor="rgba(34,211,238,0)" /></radialGradient></defs>
    <ellipse id="p10-g1" cx="680" cy="45" rx="205" ry="110" fill="url(#p10-rg1)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 12, zIndex: 10 }}>
    <span style={{ fontSize: 17.5, fontWeight: 700, color: '#ffffff' }}>HR Analysis</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
      <span style={{ padding: '4px 12px', background: 'rgba(139,92,246,0.16)', color: '#c4b5fd', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>Sep 2024</span>
      <span style={{ padding: '4px 10px', background: 'rgba(34,211,238,0.12)', color: '#67e8f9', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>View Repo -&gt;</span>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 8, background: 'rgba(15,14,28,0.62)', borderRadius: 14, padding: '14px 18px', border: '1px solid rgba(148,163,184,0.14)', zIndex: 10, flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Built an HR reporting system in Power BI to provide comprehensive workforce analysis and insights.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#a78bfa', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Utilized Power Query to clean, transform, and prepare employee datasets for accurate reporting.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Developed KPI-driven dashboards to optimize HR decision-making and monitor workforce performance.</span></div>
  </div>
</div>
```

```aura width=800 height=215 link="https://github.com/MostafaOsama0/Coffee-shop-Project"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 18, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.24)', padding: '20px 26px' }}>
  <style>{`
    @keyframes p11-o { 0%, 100% { transform: translate(0, 0); opacity: 0.4; } 50% { transform: translate(-20px, -12px); opacity: 0.72; } }
    #p11-g1 { animation: p11-o 9.1s ease-in-out infinite; }
  `}</style>
  <svg width="800" height="215" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="p11-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(79,70,229,0.44)" /><stop offset="70%" stopColor="rgba(79,70,229,0)" /></radialGradient></defs>
    <ellipse id="p11-g1" cx="120" cy="180" rx="205" ry="110" fill="url(#p11-rg1)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 12, zIndex: 10 }}>
    <span style={{ fontSize: 17.5, fontWeight: 700, color: '#ffffff' }}>Coffee Shop Analytics</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
      <span style={{ padding: '4px 12px', background: 'rgba(139,92,246,0.16)', color: '#c4b5fd', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>Oct 2024</span>
      <span style={{ padding: '4px 10px', background: 'rgba(34,211,238,0.12)', color: '#67e8f9', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>View Repo -&gt;</span>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 8, background: 'rgba(15,14,28,0.62)', borderRadius: 14, padding: '14px 18px', border: '1px solid rgba(148,163,184,0.14)', zIndex: 10, flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Created a Power BI dashboard to analyze coffee shop sales performance and customer behavior.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#a78bfa', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Utilized Power Query for data preprocessing, cleaning, and transformation.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Visualized product trends and customer preferences to identify growth opportunities and improve sales strategies.</span></div>
  </div>
</div>
```

```aura width=800 height=215 link="https://github.com/MostafaOsama0/Bike-Store-Project"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#07070d', borderRadius: 18, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(34,211,238,0.24)', padding: '20px 26px' }}>
  <style>{`
    @keyframes p12-o { 0%, 100% { transform: translate(0, 0); opacity: 0.4; } 50% { transform: translate(22px, 12px); opacity: 0.72; } }
    #p12-g1 { animation: p12-o 9.3s ease-in-out infinite; }
  `}</style>
  <svg width="800" height="215" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="p12-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(139,92,246,0.42)" /><stop offset="70%" stopColor="rgba(139,92,246,0)" /></radialGradient></defs>
    <ellipse id="p12-g1" cx="690" cy="180" rx="205" ry="110" fill="url(#p12-rg1)" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between', marginBottom: 12, zIndex: 10 }}>
    <span style={{ fontSize: 17.5, fontWeight: 700, color: '#ffffff' }}>Bike Store Project</span>
    <div style={{ display: 'flex', alignItems: 'center', gap: 8 }}>
      <span style={{ padding: '4px 12px', background: 'rgba(139,92,246,0.16)', color: '#c4b5fd', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>Aug 2024</span>
      <span style={{ padding: '4px 10px', background: 'rgba(34,211,238,0.12)', color: '#67e8f9', borderRadius: 100, fontSize: 11, fontWeight: 600 }}>View Repo -&gt;</span>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 8, background: 'rgba(15,14,28,0.62)', borderRadius: 14, padding: '14px 18px', border: '1px solid rgba(148,163,184,0.14)', zIndex: 10, flex: 1, justifyContent: 'center' }}>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Conducted sales and customer analysis for a bike store using Excel to uncover performance insights.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#a78bfa', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Applied advanced Excel functions for data filtering, transformation, and trend identification.</span></div>
    <div style={{ display: 'flex', gap: 8 }}><span style={{ color: '#22d3ee', fontSize: 12.5 }}>•</span><span style={{ fontSize: 12.2, color: '#e2e8f0', lineHeight: 1.42 }}>Designed visual reports and charts to showcase revenue patterns, customer demographics, and purchasing behavior.</span></div>
  </div>
</div>
```

```aura width=800 height=150
<div style={{ position: 'relative', display: 'flex', flexDirection: 'row', alignItems: 'center', justifyContent: 'space-between', width: '100%', height: '100%', background: '#07070d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(139,92,246,0.26)', padding: '22px 28px' }}>
  <style>{`
    @keyframes ed-o { 0%, 100% { transform: translate(0, 0); opacity: 0.45; } 50% { transform: translate(26px, -12px); opacity: 0.8; } }
    #ed-g1 { animation: ed-o 8.5s ease-in-out infinite; }
    #ed-g2 { animation: ed-o 10.5s ease-in-out infinite reverse; }
  `}</style>
  <svg width="800" height="150" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ed-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(139,92,246,0.48)" /><stop offset="70%" stopColor="rgba(139,92,246,0)" /></radialGradient>
      <radialGradient id="ed-rg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.4)" /><stop offset="70%" stopColor="rgba(34,211,238,0)" /></radialGradient>
    </defs>
    <ellipse id="ed-g1" cx="120" cy="120" rx="200" ry="100" fill="url(#ed-rg1)" />
    <ellipse id="ed-g2" cx="690" cy="30" rx="200" ry="100" fill="url(#ed-rg2)" />
  </svg>

  <div style={{ display: 'flex', flexDirection: 'column', zIndex: 10 }}>
    <span style={{ fontSize: 11, fontWeight: 700, color: '#67e8f9', letterSpacing: 2.5, textTransform: 'uppercase', marginBottom: 8 }}>Education</span>
    <span style={{ fontSize: 20, fontWeight: 700, color: '#ffffff' }}>Bachelor of Computer Science</span>
    <span style={{ fontSize: 13.5, color: '#cbd5e1', marginTop: 6 }}>Benha National University, Obour, Qalyubia, Egypt</span>
  </div>

  <div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', padding: '14px 22px', background: 'rgba(15,14,28,0.7)', borderRadius: 14, border: '1px solid rgba(139,92,246,0.3)', zIndex: 10 }}>
    <span style={{ fontSize: 10, color: '#a5b4fc', letterSpacing: 1.8, textTransform: 'uppercase' }}>Expected Graduation</span>
    <span style={{ fontSize: 24, fontWeight: 700, color: '#67e8f9', marginTop: 4 }}>2027</span>
  </div>
</div>
```

```aura width=800 height=140
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#07070d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', border: '1px solid rgba(34,211,238,0.28)', padding: '20px 34px' }}>
  <style>{`
    @keyframes ct-o1 { 0%, 100% { transform: translate(0, 0); opacity: 0.5; } 50% { transform: translate(30px, -12px); opacity: 0.85; } }
    @keyframes ct-o2 { 0%, 100% { transform: translate(0, 0); opacity: 0.45; } 50% { transform: translate(-26px, 12px); opacity: 0.8; } }
    #ct-g1 { animation: ct-o1 8s ease-in-out infinite; }
    #ct-g2 { animation: ct-o2 10s ease-in-out infinite 0.5s; }
  `}</style>
  <svg width="800" height="140" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ct-rg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(139,92,246,0.52)" /><stop offset="70%" stopColor="rgba(139,92,246,0)" /></radialGradient>
      <radialGradient id="ct-rg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(34,211,238,0.48)" /><stop offset="70%" stopColor="rgba(34,211,238,0)" /></radialGradient>
    </defs>
    <ellipse id="ct-g1" cx="150" cy="115" rx="220" ry="105" fill="url(#ct-rg1)" />
    <ellipse id="ct-g2" cx="650" cy="25" rx="220" ry="105" fill="url(#ct-rg2)" />
  </svg>

  <span style={{ fontSize: 20, fontWeight: 700, color: '#ffffff', zIndex: 10 }}>Let's Connect!</span>
  <span style={{ fontSize: 13.5, color: '#cbd5e1', textAlign: 'center', marginTop: 10, lineHeight: 1.5, zIndex: 10 }}>
    I'm open to collaboration on exciting data projects or new opportunities. Let's connect on LinkedIn or feel free to reach out via email!
  </span>
</div>
```

```aura width=192 height=46 link="https://www.linkedin.com/in/mostafaosama0/" inline align=center
<div style={{ position: 'relative', display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', padding: '0 6px', fontFamily: 'Inter, sans-serif' }}>
  <svg width="192" height="46" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <linearGradient id="fbtn-li-grad" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stopColor="#38bdf8" />
        <stop offset="50%" stopColor="#8b5cf6" />
        <stop offset="100%" stopColor="#22d3ee" />
        <animateTransform attributeName="gradientTransform" type="rotate" from="0 0.5 0.5" to="360 0.5 0.5" dur="4.5s" repeatCount="indefinite" />
      </linearGradient>
    </defs>
    <rect x="7" y="1" width="178" height="44" rx="13" fill="rgba(14,22,38,0.94)" stroke="url(#fbtn-li-grad)" strokeWidth="1.6" />
    <g transform="translate(28, 13) scale(0.84)">
      <path fill="#38bdf8" d="M19 3a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h14m-.5 15.5v-5.3a3.26 3.26 0 0 0-3.26-3.26c-.85 0-1.84.52-2.28 1.3v-1.11h-2.79v8.37h2.79v-4.93c0-.77.62-1.4 1.39-1.4a1.4 1.4 0 0 1 1.4 1.4v4.93h2.75M6.88 8.56a1.68 1.68 0 0 0 1.68-1.68c0-.93-.75-1.69-1.68-1.69a1.69 1.69 0 0 0-1.69 1.69c0 .93.76 1.68 1.69 1.68m1.39 9.94v-8.37H5.5v8.37h2.77z" />
    </g>
  </svg>
  <span style={{ fontSize: 13, fontWeight: 600, color: '#f8fafc', marginLeft: 24 }}>LinkedIn Profile</span>
</div>
```

```aura width=210 height=46 link="mailto:mostafaosama7213@gmail.com" inline align=center
<div style={{ position: 'relative', display: 'flex', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', padding: '0 6px', fontFamily: 'Inter, sans-serif' }}>
  <svg width="210" height="46" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <linearGradient id="fbtn-em-grad" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stopColor="#f472b6" />
        <stop offset="50%" stopColor="#8b5cf6" />
        <stop offset="100%" stopColor="#fb7185" />
        <animateTransform attributeName="gradientTransform" type="rotate" from="0 0.5 0.5" to="360 0.5 0.5" dur="4.5s" repeatCount="indefinite" />
      </linearGradient>
    </defs>
    <rect x="7" y="1" width="196" height="44" rx="13" fill="rgba(26,12,28,0.94)" stroke="url(#fbtn-em-grad)" strokeWidth="1.6" />
    <g transform="translate(36, 13) scale(0.84)">
      <path fill="#fb7185" d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4-8 5-8-5V6l8 5 8-5v2z" />
    </g>
  </svg>
  <span style={{ fontSize: 13, fontWeight: 600, color: '#f8fafc', marginLeft: 24 }}>Send an Email</span>
</div>
```
