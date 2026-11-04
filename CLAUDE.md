# Instruções para o Claude

Este repositório é uma central de pesquisas pessoais. Responda sempre em português.

## Quando o usuário mandar uma pesquisa

1. **Entenda o pedido**: é um tema para pesquisar, ou material dele para organizar?
   - Tema → pesquise na web (cite as fontes com link) e escreva a síntese.
   - Material próprio → organize, resuma e preserve o conteúdo original na seção "Material original".
2. **Crie o arquivo** `pesquisas/AAAA-MM-DD-titulo-em-kebab-case.md` a partir de
   `pesquisas/_modelos/pesquisa.md`. Use a data de hoje.
3. **Anexos** (PDF, imagens, planilhas) vão para `anexos/AAAA-MM-DD-titulo/` e são
   referenciados no arquivo da pesquisa.
4. **Atualize** `pesquisas/INDICE.md` adicionando uma linha no topo da tabela.
5. **Commit e push** com a mensagem `pesquisa: <título>`.
6. Responda ao usuário com um resumo curto e o caminho do arquivo.

## Regras

- Uma pesquisa por arquivo. Se o tema já existe, atualize o arquivo existente em
  vez de criar outro (e registre a atualização no histórico do arquivo).
- Separe claramente **fatos com fonte** de **opiniões/conclusões**.
- Não invente fontes. Se não encontrar, diga.
- Tags em minúsculas, sem acento, separadas por vírgula.
- Não mexa em `_legado/`.
