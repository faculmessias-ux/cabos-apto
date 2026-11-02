# Cabos Apto — GitHub Pages / PWA

## Publicação
1. Crie um repositório **público** no GitHub (ex.: `cabos-apto`).
2. Envie **todos os arquivos e a pasta `icons/` desta pasta** para a raiz do repositório.
3. Vá em **Settings → Pages → Build and deployment → Source: Deploy from a branch**.
4. Selecione **main** e **/(root)**, depois **Save**.
5. Acesse `https://SEU-USUARIO.github.io/cabos-apto/` (ajuste usuário e nome do repositório).

## Adicionar à tela inicial
- Android Chrome: abra a URL HTTPS → menu ⋮ → **Instalar app** ou **Adicionar à tela inicial**.
- Samsung Internet: abra a URL → menu → **Adicionar página a** → **Tela inicial** (rótulo pode variar).
- iPhone: abra no Safari → Compartilhar → **Adicionar à Tela de Início**.

## Armazenamento e limites
- Os dados são salvos no `localStorage` **de cada navegador/aparelho**. Não sincronizam entre celulares.
- No código original a sincronização dependia de `window.claude.use('db')`, que não existe no GitHub Pages.
- Use **Dados → Backup JSON** periodicamente e a opção Restaurar ao trocar de aparelho. Não publique backups JSON com dados internos no repositório.
- O shell básico funciona offline após o primeiro carregamento, mas **gerar PDF/Excel** exige conexão na primeira utilização para baixar bibliotecas externas (jsPDF e SheetJS); fontes externas também dependem da rede.
- Não configure credenciais privadas de bancos de dados diretamente neste repositório público. Para compartilhamento/sincronização real, implemente autenticação e regras de acesso num backend (ex.: Firebase).
