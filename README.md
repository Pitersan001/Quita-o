# Quita-o — site institucional

Site responsivo da Quita-o, assessoria veicular independente.

## Estrutura

- `public/index.html`: site completo (HTML, CSS e JavaScript).
- Formulário de primeiro contato que prepara a mensagem e abre o WhatsApp.
- Número configurado: `11959329691`.
- Sem banco de dados: os dados do formulário não são enviados a um servidor; o visitante revisa a mensagem no WhatsApp antes de enviar.

## Publicar na Cloudflare

O projeto é estático e pode ser publicado na Cloudflare Pages conectado ao GitHub.

1. Acesse https://dash.cloudflare.com/ e abra **Workers & Pages**.
2. Escolha **Create application** → **Pages** → **Import an existing Git repository**.
3. Conecte o GitHub e selecione `Pitersan001/Quita-o`.
4. Configure:
   - Production branch: `main`
   - Framework preset: `None`
   - Build command: deixe vazio (ou `exit 0`)
   - Build output directory: `public`
5. Clique em **Save and Deploy**.

Depois disso, novos commits na branch `main` acionam novas publicações. Configure domínio próprio em **Custom domains**, se desejar.

## Personalização antes de divulgar

- Confirme o nome comercial e o número de WhatsApp no arquivo `public/index.html`.
- Revise Política de Privacidade e Termos com orientação jurídica, incluindo identificação e contato do controlador dos dados.
- Atualize descrição, redes sociais e metadados.
- O site deixa claro que a assessoria é independente e não promete descontos ou resultados.

## Imagens

O layout inicial usa uma composição gráfica CSS como fallback visual. A geração da fotografia automotiva pelo Runway não foi concluída nesta etapa porque o espaço de trabalho conectado estava sem créditos. Assim que houver créditos disponíveis, gerar uma imagem automotiva original e adicioná-la em `public/assets/`, atualizando o CSS da seção hero.
