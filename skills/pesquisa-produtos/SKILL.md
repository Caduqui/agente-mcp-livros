# Skill: pesquisa de produtos

## Objetivo

Pesquisar produtos em um site de vendas e gerar um resumo em Markdown com os dados encontrados e as fontes consultadas.

## Entradas

- **Site:** URL do site de vendas.
- **Termos de busca:** um ou mais nomes, produtos ou expressões a pesquisar.
- **Filtros (opcionais):** critérios como categoria, faixa de preço, marca ou disponibilidade.
- **Quantidade de resultados:** máximo desejado por termo de busca.

## Passo a passo

1. Acesse o site informado e identifique se há um campo de busca.
2. Se houver campo de busca, pesquise cada termo e aplique os filtros fornecidos, se disponíveis.
3. Se não houver campo de busca ou não houver resultado útil, identifique e navegue pela categoria mais provável para o termo. Não percorra categorias sem relação com a busca.
4. Se ainda não houver resultados, consulte no máximo cinco páginas do catálogo, seguindo a paginação do site. Pare ao encontrar resultados suficientes ou ao atingir a quinta página; não continue a varredura.
5. Para cada produto encontrado, até a quantidade solicitada por termo, registre o título, preço, disponibilidade, avaliação e categoria. Consulte a página individual do produto quando necessário para confirmar os dados e obter a descrição.
6. Para o primeiro resultado de cada termo, escreva um resumo de duas ou três linhas da descrição, em português. Se a descrição não estiver disponível, registre isso explicitamente em vez de inferi-la.
7. Se não encontrar o produto dentro das etapas e limites acima, registre “não encontrado” e informe onde procurou, incluindo categorias e páginas verificadas.
8. Gere o arquivo Markdown de saída com os resultados, o método de busca e as fontes consultadas.

## Regras

- Não invente nem infira resultados, preços, avaliações, disponibilidade, categorias ou descrições. Registre apenas dados visíveis nas páginas consultadas.
- Não registre dados pessoais de vendedores. Inclua somente informações do produto pertinentes à pesquisa.
- Respeite o limite de cinco páginas do catálogo. A navegação por páginas de resultados de busca ou por uma categoria não autoriza percorrer o catálogo inteiro.
- Não exceda a quantidade de resultados solicitada por termo.
- Diferencie claramente “não encontrado” de resultado indisponível ou de informação que o site não fornece.
- Preserve moeda, escala de avaliação e rótulos de disponibilidade apresentados pelo site, esclarecendo-os quando forem traduzidos.
- Inclua links para as páginas dos produtos e informe a categoria e as páginas consultadas para que a busca seja verificável.

## Formato do arquivo de saída

Salve a pesquisa em um arquivo `.md` com:

1. Um título e os metadados básicos (site e data da consulta).
2. Uma nota breve explicando a estratégia de busca e os filtros usados.
3. Uma seção por termo de busca, com:
   - Uma tabela contendo **Título**, **Preço**, **Disponibilidade**, **Avaliação** e **Categoria** para cada produto encontrado.
   - Um resumo em português, de duas ou três linhas, para o primeiro resultado.
   - Ou a indicação **“Não encontrado”** e os locais/páginas consultados, se não houver resultado.
4. Links para as páginas dos produtos e, quando útil, para as páginas de categoria pesquisadas.
