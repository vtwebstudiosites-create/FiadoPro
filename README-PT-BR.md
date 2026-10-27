# FiadoPro para Android — projeto inicial

Este pacote transforma a versão HTML existente em um app Android nativo-wrapper (WebView), com nome próprio, ícone de lançador gerado pelo Android Studio, abertura de links de WhatsApp fora do app e suporte a seleção de arquivo para restauração de backup.

## Melhorias incluídas
- Mantém as funções já existentes no FiadoPro HTML.
- Aumenta letras e áreas de toque para facilitar o uso por uma pessoa idosa.
- Remove dependência de fontes remotas para o app funcionar sem internet na interface principal.
- Mantém armazenamento local do navegador WebView no aparelho.
- Permite selecionar arquivos de backup para restauração.

## Limitação importante
**Este pacote ainda não contém um APK compilado nem sincronização em nuvem.** Neste ambiente não há Android SDK/Gradle instalado para gerar e testar um APK final. Os dados continuam locais neste estágio; nuvem exige configurar um backend e autenticação, e não deve ser simulada com uma simples cópia de dados.

## Como gerar o APK
1. Instale o Android Studio em um computador.
2. Abra a pasta `FiadoPro_Android` no Android Studio.
3. Aceite instalar os componentes de SDK sugeridos pelo Android Studio.
4. Aguarde a sincronização do Gradle.
5. Use **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
6. O APK de teste normalmente fica em `app/build/outputs/apk/debug/app-debug.apk`.
7. Transfira o APK para o Android, abra o arquivo e permita a instalação para essa origem se o sistema pedir.

## Antes de usar com dívidas reais
- Testar compras, pagamentos parciais, estornos, quitação, backup e restauração no aparelho-alvo.
- Fazer cópia de segurança antes de importar ou restaurar.
- Configurar a nuvem com regras de acesso por usuário, HTTPS e backups; nunca colocar uma chave administrativa do backend dentro do HTML.
- Para recuperar dados ao trocar de aparelho, configurar e testar sincronização real antes de depender dela.

## Requisitos técnicos
- Android Studio recente.
- Android SDK 35 (instalado pelo Android Studio).
- Java/JDK compatível com a versão de Android Gradle Plugin.
