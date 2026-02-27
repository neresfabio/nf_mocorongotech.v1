# Mocorongo Tech — Modernização Essencial de Sites 🚀

Um site estático simples com foco em apresentação comercial — pronto para hospedagem estática (GitHub Pages, Netlify, Vercel ou qualquer servidor de arquivos). Projeto em português com objetivo de modernizar sites locais rapidamente: clareza, contato e confiança.

## Ícones / Atalhos
- 📱 Mobile-first
- ⚙️ Simples de manter
- 🔎 SEO básico pronto
- 🛠️ Fácil de editar
- 🌐 Pronto para deploy estático

## Estrutura do repositório
- index.html — Página principal (todo o site é aqui)
- robots.txt — Instruções para mecanismos de busca
- CNAME — (Opcional) domínio personalizado para GitHub Pages
- .nojekyll — Impede processamento Jekyll em GitHub Pages

> Observação: o arquivo `manifesto.md` é citado no HTML mas não está presente no repositório. Se quiser, adicione um `manifesto.md` com o conteúdo do manifesto.

## O que este projeto entrega
- Página única (home) com chamadas para ação (CTA) e contato por WhatsApp
- Metadados para SEO (title, description, Open Graph, Twitter Card)
- JSON-LD básico de organização
- Layout responsivo e minimalista com CSS embutido

## Pré-requisitos para rodar localmente
Nenhuma dependência especial — basta um navegador. Para servir localmente (recomendado) você pode usar um servidor HTTP simples:

- Com Python 3:
  - Na raiz do projeto: python3 -m http.server 8000
  - Acesse: http://localhost:8000

- Com Node (se preferir usar um servidor estático):
  - Instale http-server: npm i -g http-server
  - Rode: http-server -c-1
  - Acesse o endereço informado (ex.: http://localhost:8080)

- Extensões do VS Code como "Live Server" também funcionam bem.

## Configuração mínima a ajustar (passo a passo)
1. Atualizar contatos e links
   - index.html: telefone/WhatsApp (busque por `wa.me` e `tel:`)
   - site e domínio em meta tags
2. Open Graph / Imagem de compartilhamento (opcional)
   - Substitua a URL comentada `og:image` por uma imagem real (recomendado 1200×630)
3. Favicon (opcional)
   - Adicione link para favicon no <head> ou remova o comentário
4. Revisar conteúdo
   - Ajuste texto da hero, serviços entregues e manifesto conforme necessário
5. SEO técnico básico
   - Conferir title/description
   - Gerar sitemap.xml (opcional)
   - Verificar robots.txt

## Deploy (exemplos rápidos)
- GitHub Pages
  1. Commit + push do repositório para GitHub
  2. Nas configurações do repo > Pages: escolha branch `main` / `/ (root)`
  3. Se usar domínio customizado, adicione `CNAME` com o domínio e configure DNS
  4. Se não usar Jekyll (por exemplo, pastas começando com `_`), mantenha `.nojekyll`

- Netlify / Vercel
  - Conecte o repositório e publique como site estático. Sem build command necessário se não houver assets pré-processados.

## Boas práticas e checklist final ✅
- [ ] Testar em dispositivos móveis (principal foco)
- [ ] Garantir CTA principal visível no mobile
- [ ] Verificar tags meta e Open Graph
- [ ] Confirmar links de contato (WhatsApp/telefone)
- [ ] Fazer backup antes de mudanças críticas

## Como editar
- Abra `index.html` em qualquer editor de texto/IDE e edite o HTML/CSS incorporado.
- O CSS está embutido no <head> para simplicidade. Se desejar separar, crie `styles.css` e atualize o <head>.

## Suporte / Contato 📨
- Dono do projeto: Mocorongo Tech
- WhatsApp: https://wa.me/5593999021532
- Website: https://www.mocorongotech.com.br

---

Se quiser, eu posso:
- Gerar um `manifesto.md` com o texto exibido em `index.html`;
- Separar o CSS em um arquivo `styles.css`;
- Adicionar um favicon e exemplo de `og-image`;
- Criar um sitemap.xml ou instruções mais detalhadas de deploy.

Diga o que prefere que eu faça a seguir.