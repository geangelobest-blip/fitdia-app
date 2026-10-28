# FitDia — PWA de musculação

Aplicativo web instalável (PWA) em português, sem dependências de build. Inclui fichas feminina ABCD e masculina ABCDE, marcação de exercícios, campo para registrar cargas, cronômetro de descanso, mobilidade, cardio e cache offline dos arquivos principais.

## Arquivos
- `index.html`: estrutura do app.
- `styles.css`: visual responsivo.
- `app.js`: treinos e interações.
- `manifest.webmanifest`: nome, ícones e modo de instalação.
- `sw.js`: cache básico para uso offline.
- `icons/`: ícones da aplicação.

## Publicar gratuitamente com GitHub Pages
1. Entre em https://github.com/ e crie uma conta, caso ainda não tenha.
2. Crie um repositório **público** chamado `fitdia-app`.
3. Envie todos os arquivos e a pasta `icons/` deste projeto para a raiz do repositório (não envie apenas o ZIP).
4. Abra **Settings → Pages**.
5. Em **Build and deployment**, selecione **Deploy from a branch**; escolha `main` e `/ (root)`; clique **Save**.
6. Aguarde a publicação. O endereço normalmente será `https://SEU-USUARIO.github.io/fitdia-app/`.
7. Abra o endereço no Chrome do Android. No menu ⋮, escolha **Instalar app** ou **Adicionar à tela inicial**.

Documentação oficial: https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages

## Testar localmente
O PWA e o service worker precisam de HTTPS ou localhost. Para testar com Python instalado, entre nesta pasta e execute `python -m http.server 8000`; abra `http://localhost:8000` no navegador. A instalação PWA deve ser testada depois de publicar em HTTPS.

## Limites desta versão
- Os botões de vídeo abrem pesquisas no YouTube, não vídeos incorporados/curados individualmente.
- Marcações e cargas são armazenadas localmente no navegador, sem conta ou sincronização entre aparelhos.
- Não há backend, analytics, notificações push ou suporte médico individualizado.
- O deploy exige que o proprietário entre na conta de hospedagem e publique os arquivos; este projeto não foi publicado automaticamente.
