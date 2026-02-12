<div id="san-valentino-special" style="background: linear-gradient(135deg, #710808 0%, #fbda05 100%); padding: 3px; border-radius: 20px; margin: 20px auto; max-width: 350px; box-shadow: 0 10px 20px rgba(0,0,0,0.3); font-family: sans-serif;">
    <div style="background: #1a1a1a; color: white; padding: 25px; border-radius: 17px; text-align: center;">
        <h2 style="margin: 0 0 10px 0; color: #fbda05; text-transform: uppercase; letter-spacing: 2px; font-size: 1.2rem;">S ❤️ A ❤️ H ❤️ I ❤️ B</h2>
        <p style="font-size: 0.8rem; opacity: 0.8; margin-bottom: 15px;">Dal Derby del 17 Maggio ad oggi:</p>
        
        <div id="timer-sahib" style="font-size: 1.3rem; font-weight: bold; background: rgba(255,255,255,0.05); padding: 15px; border-radius: 10px; border: 1px dashed #fbda05; color: #fff; min-height: 1.5rem;">
            Caricamento...
        </div>

        <p style="margin-top: 15px; font-size: 0.85rem; color: #fbda05; font-weight: bold;">Sei il mio trofeo più bello. 🐺</p>
    </div>
</div>

<script>
    (function() {
        // Data fissata: 17 Maggio 2025
        const dataInizio = new Date(2025, 4, 17, 0, 0, 0); 

        function aggiorna() {
            const ora = new Date();
            const diff = ora - dataInizio;

            const d = Math.floor(diff / (1000 * 60 * 60 * 24));
            const h = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const m = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
            const s = Math.floor((diff % (1000 * 60)) / 1000);

            const display = document.getElementById("timer-sahib");
            if (display) {
                display.innerHTML = d + "g " + h + "o " + m + "m " + s + "s";
            }
        }
        setInterval(aggiorna, 1000);
        aggiorna();
    })();
</script>
