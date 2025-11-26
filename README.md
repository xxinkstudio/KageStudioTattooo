<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Kage Triple Ink</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: Arial, Helvetica, sans-serif;
      background: #000;
      color: #fff;
      line-height: 1.6;
    }
    .page {
      max-width: 820px;
      margin: 0 auto;
      padding: 40px 20px;
    }
    h1 {
      font-size: 48px;
      font-weight: 900;
      margin-bottom: 20px;
      text-transform: uppercase;
      letter-spacing: 2px;
    }
    h2 {
      margin-top: 40px;
      font-size: 28px;
      font-weight: 700;
    }
    p, li {
      font-size: 18px;
      margin-bottom: 16px;
    }
    .button {
      display: inline-block;
      background: #fff;
      color: #000;
      padding: 16px 28px;
      border-radius: 6px;
      font-size: 20px;
      font-weight: bold;
      text-decoration: none;
      margin-top: 20px;
    }
    .box {
      background: #111;
      padding: 20px;
      border-radius: 10px;
      margin: 25px 0;
    }
    ul {
      padding-left: 20px;
    }
    /* botão fixo do rodapé (visível em dispositivos móveis e desktop) */
    .fixed-cta{
      position:fixed;
      bottom:0;
      left:0;
      right:0;
      background:#fff;
      color:#000;
      padding:16px;
      text-align:center;
      font-size:18px;
      font-weight:700;
      text-decoration:none;
      z-index:999;
    }
    /* espaço extra no final do conteúdo para não ficar atrás do botão fixo */
    .spacer{height:76px}
  </style>
</head>
<body>
  <div class="page">
    <img src="logo.png" alt="Logo Kage Studio" style="width:140px; margin-bottom:20px; display:block;">
    <h1>Kage Triple Ink</h1>
    <p>3 tatuagens blackwork de 6 a 8 cm por um preço único. Agende como quiser. Use até março/26. Presenteie quem você quiser.<br><br></p>

    <div class="box" style="text-align:center; font-size:22px; font-weight:bold;">Promoção válida por: <span id="countdown" style="color:#0f0;"></span></div>
    <a href="https://wa.me/5521981130991" class="button">Garantir meu pacote</a>

    <h2>O que é o Kage Triple Ink?</h2>
    <p>Uma oferta especial do Kage Studio para quem quer tatuar com flexibilidade, qualidade e liberdade. Você compra agora, agenda depois e usa no seu ritmo — até março de 2026.</p>

    <div class="box">
      <h2>Como funciona</h2>
      <ul>
        <li>Você compra o pacote com 3 tatuagens.</li>
        <li>Agenda cada sessão separadamente, quando quiser.</li>
        <li>Pode usar até 31/03/2026.</li>
        <li>Pode fazer as 3 no mesmo dia, se quiser.</li>
        <li>Pode dar de presente para outra pessoa.</li>
      </ul>
    </div>

    <div class="box">
      <h2>Regras</h2>
      <ul>
        <li>Válido exclusivamente para tattoos de 6–8 cm.</li>
        <li>Transferível somente antes da ativação.</li>
      </ul>
    </div>

    <h2>Por que aproveitar agora?</h2>
    <p>Essa campanha tem um preço promocional que poderá mudar a qualquer momento! Esse é um pacote limitado e que pode acabar a qualquer momento! Aproveite agora!</p>
    
    <p><strong style="font-size:28px; color:#0f0;">Valor: R$ 400,00</strong></p>

    <a href="https://wa.me/5521981130991" class="button">Quero garantir agora</a>

    <div class="box" style="text-align:center; font-size:22px; font-weight:bold;">Promoção válida por: <span id="countdown2" style="color:#0f0;"></span></div>

    <p style="margin-top: 60px; opacity: 0.6; font-size: 14px;">Todos os direitos reservados a Kage Studio Tattoo e seu fundador Gabriel Diogo dos Santos. Cascadura/RJ</p>

    <div class="spacer"></div>
  </div>

  <!-- Scripts colocados ao final da página e executados após o DOM estar pronto -->
  <script>
    document.addEventListener('DOMContentLoaded', () => {
      const targetTime = new Date('2025-12-31T23:59:59').getTime();

      function updateCountdownTo(target, elementId) {
        const el = document.getElementById(elementId);
        if (!el) return; // elemento não existe — evita erro
        const now = Date.now();
        const diff = target - now;
        if (diff <= 0) { el.innerHTML = 'Encerrado'; return; }
        const d = Math.floor(diff / (1000*60*60*24));
        const h = Math.floor((diff % (1000*60*60*24)) / (1000*60*60));
        const m = Math.floor((diff % (1000*60*60)) / (1000*60));
        const s = Math.floor((diff % (1000*60)) / 1000);
        el.innerHTML = `${d}d ${h}h ${m}m ${s}s`;
      }

      // Atualiza imediatamente e depois a cada segundo
      updateCountdownTo(targetTime, 'countdown');
      updateCountdownTo(targetTime, 'countdown2');
      setInterval(() => {
        updateCountdownTo(targetTime, 'countdown');
        updateCountdownTo(targetTime, 'countdown2');
      }, 1000);
    });
  </script>

  <a href="https://wa.me/5521981130991" class="fixed-cta">Garantir pacote agora</a>
</body>
</html>
