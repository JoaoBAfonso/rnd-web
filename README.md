# CymaForma RND (web)

Controlador web/PWA para o RND. Usa Web MIDI com SysEx (Chrome ou Edge) e funciona offline depois de instalado.

## Publicar no GitHub Pages

1. Cria um repositório novo no GitHub (por exemplo `rnd-web`).
2. Nesta pasta:

   ```powershell
   git init -b main
   git add .
   git commit -m "CymaForma RND web"
   git remote add origin https://github.com/<utilizador>/rnd-web.git
   git push -u origin main
   ```

3. No GitHub: Settings > Pages > Source: "Deploy from a branch", branch `main`, pasta `/ (root)`.
4. Passado cerca de um minuto, a app fica em `https://<utilizador>.github.io/rnd-web/`.

## Instalar no Android

1. Abre o endereço acima no Chrome do telemóvel (com internet, uma vez).
2. Menu do Chrome > "Instalar app" (ou "Adicionar ao ecrã principal").
3. Liga o RND por USB/OTG, abre a app e toca em "Ligar MIDI". Aceita a permissão de MIDI/SysEx.

Depois disto a app abre offline. Quando houver rede, atualiza-se sozinha; se mudares ficheiros, aumenta a versão `CACHE` em `sw.js`.

## Teste local

`powershell -ExecutionPolicy Bypass -File serve.ps1` e abre `http://localhost:8080`.
