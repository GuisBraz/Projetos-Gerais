# Projetos-Gerais

Plataforma de exposição dos meus projetos: ferramentas técnicas de caldeiraria e solda, software de produção e materiais de estudo, todos acessíveis a partir de uma página só.

**Site:** https://guisbraz.github.io/Projetos-Gerais/

## Estrutura

```
index.html            → a plataforma (catálogo de projetos)
assets/capas/         → imagens de capa dos cards
guia-tecnico/         → Guia Técnico         (veio do repo GuisBraz/calculadora-peso)
```

Os projetos que ficam em pastas deste repositório abrem na mesma aba. Os independentes (PROJTEC 1D, ROSTAG PCP, Faculdade de Bolso — que inclui a Escola de Usinagem — e Portfólio) continuam nos próprios repositórios e são só linkados daqui.

## Adicionar um projeto

1. **Projeto hospedado aqui:** crie uma pasta (ex.: `novo-site/`) com o `index.html` dentro. Use caminhos relativos (`style.css`, `./img/logo.png`), nunca começando com `/`.
2. Abra o `index.html` da raiz e acrescente um objeto na lista `PROJETOS`:

```js
{
  id: 'novo-site', codigo: 'PG-06', local: true, categoria: 'ferramentas',
  titulo: 'Nome do projeto',
  status: 'Ativo',
  descricao: 'Uma frase dizendo o que ele faz.',
  destaques: ['Ponto 1', 'Ponto 2', 'Ponto 3'],
  tecnologia: 'HTML · JavaScript',
  url: 'novo-site/', capa: 'assets/capas/novo-site.jpg',
  busca: 'palavras extras para a busca',
},
```

Categorias: `ferramentas`, `software`, `estudos`, `pessoal`. Para um projeto de outro repositório, use `local: false` e a URL completa.

---
ROSTAG Soluções · Guilherme dos Santos Braz
