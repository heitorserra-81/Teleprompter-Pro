# TILO — Teleprompter Pro

PWA de teleprompter em português, desenvolvido por Heitor.

## Como testar localmente
A câmera e o microfone exigem contexto seguro: HTTPS ou `localhost`.
- Abra um terminal nesta pasta.
- Execute `python -m http.server 8000`.
- Acesse `http://localhost:8000`.

## Publicar no GitHub Pages
1. Crie um repositório no GitHub.
2. Envie todos os arquivos desta pasta para a raiz do repositório.
3. Em **Settings → Pages**, escolha a branch principal e a pasta `/ (root)`.
4. Aguarde a publicação e abra o endereço HTTPS gerado.

## Instalação
No Chrome/Edge, abra o site publicado e use **Instalar app** ou o ícone de instalação na barra de endereço. No celular, abra no navegador e escolha **Adicionar à tela inicial**.

## Recursos incluídos
- PWA instalável e cache offline básico.
- Pré-visualização de câmera e gravação de áudio/vídeo pelo navegador.
- Roteiro editável, controles de fonte, cor, tamanho e formatação básica.
- Rolagem automática, velocidade, transparência, posição, espelhamento e tela cheia.

## Limitações importantes
- A gravação usa `MediaRecorder` e normalmente gera WebM; suporte varia conforme navegador/dispositivo.
- Câmera e microfone precisam de permissão e HTTPS (localhost é exceção).
- A formatação do editor nesta primeira versão é básica: os botões aplicam marcações no texto selecionado, não um editor rico completo por palavra. O vídeo grava o fluxo da câmera; a sobreposição do roteiro na prévia não é composta automaticamente no arquivo gravado nesta versão.
