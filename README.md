<!DOCTYPE html>
if (diff <= 0) {
document.getElementById(id).innerHTML = 'Encerrado';
return;
}


const d = Math.floor(diff / (1000*60*60*24));
const h = Math.floor((diff % (1000*60*60*24)) / (1000*60*60));
const m = Math.floor((diff % (1000*60*60)) / (1000*60));
const s = Math.floor((diff % (1000*60)) / 1000);


document.getElementById(id).innerHTML = `${d}d ${h}h ${m}m ${s}s`;
}


setInterval(() => {
updateCountdown('countdown');
updateCountdown('countdown2');
}, 1000);
});
</script>


<div class="page">
<img src="assets/logo.png" alt="Logo Kage Studio" style="width:140px; margin-bottom:20px; display:block;">


<h1>Kage Triple Ink</h1>
<p>3 tatuagens blackwork de 6 a 8 cm por um preço único. Agende como quiser. Use até março/26. Presenteie quem você quiser.</p>


<div class="count-box">
Promoção válida por: <span id="countdown" style="color:#0f0;"></span>
</div>


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


<p style="font-size:20px; color:#ccc; margin-bottom:25px;">
Essa campanha tem um preço promocional que poderá mudar a qualquer momento!<br>
Esse é um pacote limitado e que pode acabar a qualquer momento!<br>
Aproveite agora!
</p>


<p><strong style="font-size:28px; color:#0f0;">Valor: R$ 400,00</strong></p>


<a href="https://wa.me/5521981130991" class="button">Quero garantir agora</a>


<div class="count-box">
Promoção válida por: <span id="countdown2" style="color:#0f0;"></span>
</div>


<p style="margin-top: 60px; opacity: 0.6; font-size: 14px;">
Todos os direitos reservados a Kage Studio Tattoo e seu fundador Gabriel Diogo dos Santos. Cascadura/RJ
</p>
</div>


<a href="https://wa.me/5521981130991" class="fixed-btn">Garantir pacote agora</a>


</body>
</html>
