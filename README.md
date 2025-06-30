<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Análise Forex em Tempo Real</title>
    <link rel="stylesheet" href="style.css">
    <link rel="manifest" href="manifest.json">
    <meta name="theme-color" content="#2c3e50"/>
</head>
<body>
    <div class="container">
        <header>
            <h1>Análise Forex Ao Vivo</h1>
            <p>Par de Moedas: <span id="pair">EUR/USD</span></p>
        </header>

        <main>
            <div class="card price-card">
                <h2>Preço Atual</h2>
                <p id="price" class="loading">Carregando...</p>
                <small id="timestamp">--</small>
            </div>

            <div class="card signal-card" id="signal-card">
                <h2>Sinal de Negociação</h2>
                <p id="signal" class="loading">Analisando...</p>
            </div>

            <div class="card indicators-card">
                <h2>Indicadores Técnicos</h2>
                <div class="indicator">
                    <p>RSI (14): <span id="rsi-value" class="loading">--</span></p>
                    <div class="progress-bar">
                        <div id="rsi-progress"></div>
                    </div>
                </div>
                <div class="indicator">
                    <p>SMA (50): <span id="sma50-value" class="loading">--</span></p>
                    <p>SMA (200): <span id="sma200-value" class="loading">--</span></p>
                </div>
            </div>

            <div class="disclaimer">
                <p><strong>Aviso Legal:</strong> Esta é uma ferramenta de demonstração e não um conselho financeiro. Use por sua conta e risco.</p>
            </div>
        </main>

        <footer>
            <button id="refresh-btn">Atualizar Agora</button>
        </footer>
    </div>
    <script src="app.js"></script>
</body>
</html>
