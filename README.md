# RC Bot · Coin-Flip (Android, sem root)

App Android (Kotlin) que joga o minijogo **Coin-Flip** do RollerCoin sozinho.

## Como funciona
- **Serviço de Acessibilidade** faz os toques (`dispatchGesture`) e lê o ecrã (`takeScreenshot`, Android 11+). Não precisa de root nem de MediaProjection.
- Um painel e uma grelha flutuantes deixam-te alinhar a grelha com os cartões.
- O bot vira um cartão, guarda uma "assinatura" visual da face (miniatura 8x8) e, quando vê o par de um cartão já conhecido, vira-o. Não repete jogadas desnecessárias.

## Compilar
1. Abre a pasta no **Android Studio** (Hedgehog ou mais recente) e deixa sincronizar o Gradle.
2. Liga o telemóvel por USB (depuração USB) e carrega em Run, ou usa Build > Build APK.

## Usar
1. Instala a app e ativa **RC Bot (Coin-Flip)** em Definições > Acessibilidade.
2. Abre o RollerCoin > Coin-Flip, com os cartões virados para baixo.
3. Arrasta os cantos amarelos da grelha até ficarem em cima dos cartões. Ajusta Lin/Col.
4. Carrega em ▶ Iniciar.

## Ajustes
- **Esp−/Esp+**: tempo de espera entre jogadas (aumenta se os cartões ainda estiverem a virar).
- `matchThr` em `CoinFlipBot.kt` (0.10): se falhar pares, baixa; se juntar cartões diferentes, também baixa. Se não reconhecer pares iguais, sobe.

## Aviso
O RollerCoin proíbe bots nos seus termos. Contas apanhadas podem ser banidas e perder o saldo. Usa por tua conta e risco.
