# Landing page · mesmapagina.com.br

Página estática (um único `index.html`, sem build, sem dependências) para sondar demanda externa
pela Mesma Página. Projeto separado da `Aplicacao/`: nada aqui importa ou depende dela.

## Objetivo do teste
Hipótese: PMs/PMOs de fora do piloto têm o mesmo problema e querem usar a ferramenta.
Sinal de sucesso (sugestão, definir antes de divulgar): N cadastros qualificados em X semanas.

## Lista de espera
- Destino: banco **Lista de espera** no Notion (campos Name, email, cargo).
- Captura: visualização **Formulário** do próprio banco, com link público.
- No `index.html`, edite apenas a variável `LINK_LISTA` (no final do arquivo).
  Enquanto ela não tiver um link `http...`, os botões rolam para o fim da página.

## Publicar (Vercel, projeto separado)
1. Vercel → Add New → Project → importe o mesmo repositório.
2. **Root Directory:** `Landing Page` · Framework Preset: **Other** · sem build command.
3. Settings → Domains → adicione `mesmapagina.com.br` e `www.mesmapagina.com.br`.
4. No registro.br, configure o DNS com os registros que a Vercel mostrar.

## Atenção
- O plano Hobby da Vercel proíbe uso comercial. Uma lista de espera para um produto pode se enquadrar; reveja o D6 antes de divulgar amplamente.
- LGPD: a página coleta nome, e-mail e cargo. Inclua no formulário do Notion uma frase dizendo para que os dados serão usados.
