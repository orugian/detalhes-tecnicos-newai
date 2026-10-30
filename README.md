# Detalhes técnicos do NewAI

Página estática que abre a arquitetura do NewAI por dentro: o que é memória, o que é
modelo, o que é motor determinístico, e como o turno de conversa percorre as camadas.

**No ar:** https://detalhes-tecnicos-newai.vercel.app

## Conteúdo

| Arquivo | Papel |
| --- | --- |
| `index.html` | a página publicada (HTML + CSS + JS inline, sem build) |
| `assets/logo-nubank.jpg` | logo usada no rodapé |
| `assets/telas/0-investimentos.png` | print da tela de investimentos |
| `assets/telas/1-cotacao.png` | print da cotação |
| `assets/telas/4-pix-credito.png` | print do Pix no crédito |
| `assets/telas/5-imposto.png` | print do imposto de renda |

As fontes (Inter Tight e JetBrains Mono) vêm do Google Fonts.

## Rodando local

Abrir `index.html` no navegador basta — não há build nem dependências. Para simular
o domínio final, sirva a pasta:

```bash
npx serve .
```

## Deploy

Projeto `detalhes-tecnicos-newai` na Vercel (time `guilherme-orugians-projects`),
repositório conectado à branch `main`: push em `main` = deploy de produção.
Site estático, sem build nem variáveis de ambiente.

```bash
vercel link --project detalhes-tecnicos-newai
vercel deploy --prod
```

## Também publicado

- Aplicação (protótipo funcional): https://desafio-nubank.vercel.app
  — código em [orugian/desafio-nubank](https://github.com/orugian/desafio-nubank).
