# auralis-website

Site estático mínimo para GitHub Pages: página institucional provisória do Auralis e páginas informativas da integração OAuth pessoal usada nos backups (Rclone + Google Drive).

## Estrutura

```
index.html                     Página do Auralis
backup-oauth/index.html        Página do aplicativo OAuth "rclone"
backup-oauth/privacy/index.html  Política de privacidade da integração
README.md
```

Somente HTML com CSS embutido. Sem JavaScript, backend, formulários, cookies, analytics, fontes ou imagens externas. Todos os links internos são relativos, então o site funciona tanto em `https://<usuario>.github.io/<repositorio>/` quanto na raiz de um domínio.

## URLs para o Google Auth Platform (Branding)

Depois de publicado, com `<base>` sendo o endereço do GitHub Pages:

- Página inicial do aplicativo: `<base>/backup-oauth/`
- Política de privacidade: `<base>/backup-oauth/privacy/`

## Publicação (somente quando autorizada)

1. Criar um repositório público no GitHub (por exemplo `auralis-website`).
2. Enviar estes arquivos para a raiz da branch `main`.
3. Em Settings → Pages: Source = "Deploy from a branch", Branch = `main`, pasta `/ (root)`.
4. Conferir as três páginas no navegador antes de usá-las no Google Cloud.

## Pendências antes de publicar

- Definir o nome do usuário/repositório GitHub, que determina as URLs finais.
- Revisar os textos.

## Regras de conteúdo

- Não incluir tokens, identificadores do cliente OAuth, nomes de remotos, caminhos locais, logs ou detalhes operacionais do backup.
- Não incluir datas de lançamento, links de loja ainda inexistentes ou imagens do jogo sem aprovação.
