# Hub do Assessor · Gustavo Amorim

Versão 2 do Hub do Assessor — ferramentas de apoio comercial para assessoria de investimentos.

**No ar:** https://gustavoamorim27-svg.github.io/hub-gustavo-amorim/

## O que tem

| Área | Ferramentas |
|---|---|
| Assessoria | Carteiras · Renda variável · Planejamento · Comparações · Diagnóstico · Rebalanceamento |
| Património | IR e DARF · Sucessão (Whole Life) · Holding patrimonial |
| Materiais | Apresentação institucional |

## Como funciona

Arquivo único (`index.html`, ~4,5 MB) com todo o CSS e JavaScript embutidos — os módulos ES vão inline como data URIs e as bibliotecas (Chart.js, SheetJS, jsPDF, html2canvas) estão empacotadas junto. Não precisa de build nem de servidor: abrir o arquivo já funciona.

A navegação usa hash router (`#/carteiras`, `#/simulador`, ...), que é o que faz as rotas funcionarem no GitHub Pages sem configuração de servidor.

Os dados ficam no `localStorage` do próprio navegador, sob o prefixo `hub:v2:`. Nada é enviado para servidor — em Preferências e dados dá para exportar e restaurar um backup em JSON.

Cotações de renda variável são buscadas no Yahoo Finance através de proxies CORS públicos, sem token. Se a rede bloquear, a interface não quebra: o preço continua editável na mão.

## Versão original

A v1 segue disponível em https://gustavoamorim27-svg.github.io/hub-assessor/

---

Material de apoio interno. Não constitui recomendação de investimento.
