# IPE Vectorized Figures for LaTeX

## Visão Geral do Projeto

Este repositório armazena figuras e diagramas vetorizados criados com o software IPE (Ipe extensible drawing editor).

O objetivo é fornecer assets em formato PDF nativo e vetorizado, garantindo:
* Resolução Independente: Escalabilidade perfeita sem perda de qualidade.
* Integração LaTeX: Textos e fórmulas são renderizados pelo motor LaTeX do seu documento, garantindo uniformidade tipográfica.

---

## Como Utilizar (LaTeX)

Use o pacote graphicx com um compilador moderno (pdflatex, lualatex).

### 1. Pacote
Adicione no preâmbulo: \usepackage{graphicx}

### 2. Inclusão
Aponte para o diretório /pdf, omitindo a extensão .pdf para flexibilidade:

\begin{figure}[h!]
    \centering
    \includegraphics[width=0.85\textwidth]{pdf/nome_do_diagrama} 
    \caption{Diagrama esquemático.}
    \label{fig:diagrama_ipe}
\end{figure}

---

## Estrutura de Diretórios

| Diretório | Conteúdo | Propósito |
| :--- | :--- | :--- |
| /pdf | Arquivos .pdf vetorizados finais. | PRONTO PARA USO. |
| /src | Arquivos fonte .ipe (XML editável). | Para modificação e manutenção. |
| /assets | Arquivos auxiliares (ex: stylesheets .isy). | Recursos de apoio. |

---

## Contribuição

Para adicionar uma figura, você deve incluir ambos os arquivos:
1. O arquivo editável .ipe em /src/.
2. O arquivo de saída .pdf exportado em /pdf/.

Abra um Pull Request (PR) com o novo par de arquivos.