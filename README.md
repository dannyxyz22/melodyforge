# 🎵 MelodyForge

Criador de melodias e frases musicais que roda inteiro no navegador — sem build, sem backend e sem instalação.

**[▶ Abrir o app no GitHub Pages](https://dannyxyz22.github.io/melodyforge/)**

## O que faz

- **Frases completas**: escolha entre 16, 32, 64 (padrão) ou 128 passos — de 1 a 8 compassos. O gerador cria um tema (A) e o desenvolve com repetição, variação leve (A′, A″) e sequências (B), em formas como `A–A′–B–A′`.
- **🔗 Combinar / variar** (tecla `X`): reagrupa os compassos da melodia atual para testar combinações diferentes.
- **Música completa**: gera estrofes, refrão e ponte com variações guardadas, harmonia lenta (2 acordes por compasso), baixo e bateria.
- **Modo vocal**: `livre`, `fácil` ou `muito fácil` — restringe as notas a um conjunto cantável, limita os saltos e cuida da cadência.
- **Piano real amostrado**: instrumento opcional via `smplr` / `SplendidGrandPiano`, com realce no mix para a melodia ficar à frente da harmonia. Se a rede falhar, volta automaticamente para o piano sintetizado.
- **Exportação**: MIDI (4 faixas), JSON e tablatura, todos acompanhando o tamanho da frase.

## Como usar

Abra a URL do GitHub Pages ou baixe `melodyforge.html` e abra no navegador. Tudo é autocontido em um único arquivo HTML.

Atalhos principais: `Espaço` play/stop · `N` nova melodia · `X` combinar/variar · `R` ritmo aleatório · `C` contorno · `M` criar música · `B` estilo vocal · `L` limpar.

## Estrutura

| Arquivo | Finalidade |
| --- | --- |
| `melodyforge.html` | App completo (UI, gerador, áudio, arranjo e exports) |
| `index.html` | Redireciona para `melodyforge.html` na raiz do Pages |

## Dependências externas

- Tailwind CSS via CDN (`gstatic.com`)
- `smplr` e samples do Splendid Grand Piano via CDN, carregados sob demanda apenas quando o instrumento "Piano Real" é selecionado

## Publicação

O GitHub Pages serve a branch `main` a partir da raiz. Qualquer push em `main` atualiza o site automaticamente.
