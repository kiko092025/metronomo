<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Presets de Gravação em Linha — Guitarra & Baixo</title>
  <style>
    :root{--bg:#0f1724;--card:#0b1220;--muted:#9aa4b2;--accent:#eab308}
    body{font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial; margin:0; background:linear-gradient(180deg,#071022 0%, #071229 60%); color:#e6eef6}
    .container{max-width:980px;margin:36px auto;padding:28px}
    header{display:flex;gap:16px;align-items:center}
    h1{margin:0;font-size:28px}
    p.lead{color:var(--muted);margin:6px 0 18px}
    .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:18px}
    .card{background:var(--card);padding:16px;border-radius:12px;box-shadow:0 6px 20px rgba(2,6,23,0.6);border:1px solid rgba(255,255,255,0.02)}
    .preset-title{display:flex;justify-content:space-between;align-items:center}
    .preset-title h2{font-size:18px;margin:0}
    .meta{color:var(--muted);font-size:13px;margin-top:6px}
    pre{background:#071021;padding:12px;border-radius:8px;overflow:auto;font-size:13px;line-height:1.5}
    button{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:8px 10px;border-radius:8px;color:#e6eef6;cursor:pointer}
    .actions{display:flex;gap:8px;margin-top:12px}
    .footer{margin-top:22px;color:var(--muted);font-size:13px}
    .hint{background:rgba(255,255,255,0.02);padding:10px;border-radius:8px;color:var(--muted);font-size:14px}
    a.link{color:var(--accent);text-decoration:none}
    @media (max-width:520px){body{padding:12px}.container{padding:12px}}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div>
        <h1>Presets — Gravação em Linha (DI)</h1>
        <p class="lead">Tom encorajador e visão tradicional: ajustes simples, sólidos e fiéis ao que sempre funcionou em estúdio. Use estes presets como ponto de partida e ajuste com o ouvido.</p>
      </div>
    </header>

    <section style="margin-top:18px">
      <div class="hint">Dica clássica: grave o sinal DI limpo e, se possível, faça uma pista paralela com saída do amp sim. Assim preserva controle para reamping no futuro.</div>
    </section>

    <main class="grid" style="margin-top:18px">

      <article class="card">
        <div class="preset-title">
          <h2>Guitarra — Limpo com Corpo</h2>
          <small class="meta">Uso: Rítmica, arpejos, comping</small>
        </div>
        <div class="meta">Mapeamento sugerido (Waves): GTR3/CLA Guitars, Renaissance Compressor, RVerb</div>
        <pre id="preset1">Amp Sim: Fender Twin / Vox AC30 (clean)
EQ:
  - Graves: 40–60%
  - Médios: 50–55% (presença)
  - Agudos: 55–60%
Compressor: leve — ataque médio, sustain 30–40%
Reverb: Plate/Spring — mix 15–20%
Chorus: opcional, leve
Notas: mantenha dinâmica; evite excesso de brilho para não cansar a mix.</pre>
        <div class="actions">
          <button onclick="copyText('preset1')">Copiar preset</button>
          <button onclick="downloadText('preset1','guitarra_limpo.txt')">Baixar .txt</button>
        </div>
      </article>

      <article class="card">
        <div class="preset-title">
          <h2>Guitarra — Crunch (Rock / Blues)</h2>
          <small class="meta">Uso: Bases, composições com drive</small>
        </div>
        <div class="meta">Mapeamento sugerido (Waves): GTR3, CLA Guitars, Abbey Road Plates, Renaissance Vox</div>
        <pre id="preset2">Amp Sim: Marshall JCM800 / Vox AC30 em drive suave
Gain: 30–40% (controle do ataque)
EQ:
  - Graves: 45%
  - Médios: 60% (corpo e presença)
  - Agudos: 55%
Compressor: leve para controle dinâmico
Reverb: Plate curto
Notas: busque o ponto onde as palhetadas ganham corpo sem embotar.</pre>
        <div class="actions">
          <button onclick="copyText('preset2')">Copiar preset</button>
          <button onclick="downloadText('preset2','guitarra_crunch.txt')">Baixar .txt</button>
        </div>
      </article>

      <article class="card">
        <div class="preset-title">
          <h2>Baixo — Firme e Definido</h2>
          <small class="meta">Uso: Linha de baixo no arranjo</small>
        </div>
        <div class="meta">Mapeamento sugerido (Waves): Bass Rider, Kramer HLS Limiter, RBass, CLA Bass</div>
        <pre id="preset3">Amp Sim: Ampeg SVT / Bassman
EQ:
  - Graves: 60% (peso)
  - Médios: 50% (definição)
  - Agudos: 40% (clareza)
Compressor: ataque rápido, sustain médio
Drive: opcional e sutil para calor
Notas: mantenha espaço para o bumbo; corte subgrave se acumular.</pre>
        <div class="actions">
          <button onclick="copyText('preset3')">Copiar preset</button>
          <button onclick="downloadText('preset3','baixo_firme.txt')">Baixar .txt</button>
        </div>
      </article>

      <article class="card">
        <div class="preset-title">
          <h2>Preset Auxiliar — DI + Reampar (Fluxo)</h2>
          <small class="meta">Uso: fluxo tradicional em estúdio</small>
        </div>
        <div class="meta">Mapeamento sugerido (Waves): GTR3 reamped; Abbey Road Reverbs; SSL Compressor</div>
        <pre id="preset4">1) Grave sinal DI limpo (canal seco)
2) Duplique pista: uma para processamento com amp sim, outra mantenha DI
3) Quando mixar, combine DI + amp sim para ajustar corpo e ataque
4) Se reamping: exporte DI e passe por amp real ou plugin em outra sessão
Notas: este método é o que os estúdios tradicionais usam para máxima flexibilidade.</pre>
        <div class="actions">
          <button onclick="copyText('preset4')">Copiar preset</button>
          <button onclick="downloadText('preset4','di_reampar.txt')">Baixar .txt</button>
        </div>
      </article>

    </main>

    <section class="card" style="margin-top:18px">
      <h3 style="margin-top:0">Mapeamento rápido para Waves (sugestões)</h3>
      <p class="meta">Se você tem a coleção Waves completa, aqui estão plugins tradicionais para cada função — comece por eles:</p>
      <ul style="color:var(--muted)">
        <li><strong>Amp Sim / Guitarra:</strong> GTR3, CLA Guitars</li>
        <li><strong>Compressão:</strong> Renaissance Compressor, SSL G-Master Buss Compressor</li>
        <li><strong>Reverb:</strong> RVerb, Abbey Road Reverb Plates</li>
        <li><strong>Baixo:</strong> CLA Bass, RBass, Bass Rider</li>
        <li><strong>Coloração / Tape / Saturação:</strong> Kramer Master Tape, J37 Tape</li>
      </ul>
      <div class="footer">Lembre-se: esses nomes são pontos de partida. Ajuste por ouvido — a tradição nos ensina que o melhor som vem de ouvir mais que de mirar números.</div>
    </section>

    <footer style="margin-top:18px;text-align:center;color:var(--muted);font-size:13px">
    </footer>
  </div>

  <script>
    function copyText(id){
      const text = document.getElementById(id).innerText;
      navigator.clipboard.writeText(text).then(()=>{
        alert('Preset copiado para a área de transferência — use com confiança!');
      },()=>{alert('Não foi possível copiar. Selecionar manualmente.')});
    }
    function downloadText(id, filename){
      const text = document.getElementById(id).innerText;
      const blob = new Blob([text], {type: 'text/plain;charset=utf-8'});
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url; a.download = filename; document.body.appendChild(a); a.click();
      setTimeout(()=>{ URL.revokeObjectURL(url); a.remove(); }, 100);
    }
  </script>
</body>
</html>
