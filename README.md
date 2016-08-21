# O que é?

É um template em LaTeX para escrever trabalhos de conclusão de curso.

Esse projeto foi desenvolvido tomando como base o [**ueceTeX2**](https://github.com/thiagodnf/uecetex2) e seguindo as normas da ABNT. As alterações posteriores tiveram o objetivo de adaptar o template para o modelo de TCC do curso de Ciência da Computação da UFRPE/UAG.

# Por onde começo?
Para utilizar o ueceTeX2 você precisa seguir os seguintes passos:

1. Clique [aqui](https://github.com/ramonsantos/template_tcc/releases/download/v1.0/template_tcc.zip) para baixar o projeto
2. Descompacte o arquivo no diretório onde vc deseja guardar os arquivos do seu trabalho
3. Crie o seu texto a partir do arquivo *documento.tex* distribuído no arquivo baixado. O arquivo possui comentários e é, em certa medida, auto-explicativo.

> Você é iniciante em LaTeX ou em abnTeX2? Clique [aqui](https://code.google.com/p/abntex2/wiki/PorOndeComecar) para acessar a página desenvolvida pela equipe do abnTeX2. Nesta página é possível acessar diversos links sobre o LaTeX e sobre o abnTeX2 como, por exemplo, a história do LaTeX e alguns minicursos desenvolvidos em outras universidades

# Como compilar?

Uma vez que todas as informações foram colocadas no documento, você precisará de um programa para compilar e gerar o PDF do seu trabalho.

### Windows
 - Acesse [https://github.com/thiagodnf/uecetex2/wiki/Como-instalar-no-Windows]

### Linux

 - Acesse [https://github.com/thiagodnf/uecetex2/wiki/Como-instalar-no-Linux]

# Dicas
Veja a seguir como inserir alguns elementos no seu texto.

### Como inserir uma Tabela
```tex
\begin{table}[h!]
	\centering
	\Caption{\label{tab:label_da_tabela} Legenda da Tabela}
	\UECEtab{}{
		\begin{tabular}{ccll}
			\toprule
				Quisque & pharetra & tempus & vulputate \\
			\midrule \midrule
				E1 & Complete coverage & Both splice sites \\
				E2 & Complete coverage & Both splice sites \\
				E3 & Partial coverage & Both splice sites & Both \\
				E4 & Partial coverage & One splice site & Both \\
				E5 & Complete or coverage & No splice & Both \\
				E6 & No coverage & No splice sites\\
			\bottomrule
		\end{tabular}
	}{
		\Fonte{Elaborado pelo autor}
    }
\end{table}
```

### Como inserir um Quadro
```tex
\begin{quadro}[h!]
	\centering
	\Caption{\label{qua:label_do_quadro} Legenda do Quadro}
	\UECEqua{}{
		\begin{tabular}{|c|c|}
			\hline
			Quisque & pharetra \\
			\hline
			E1 & Complete coverage  \\
			\hline
			E2 & Complete coverage \\
			\hline
		\end{tabular}
	}{
		\Fonte{Elaborado pelo autor}
	}
\end{quadro}
```

### Como inserir uma figura
```tex
\begin{figure}[h!]
	\centering
	\Caption{\label{fig:label_da_figura} Legenda da Figura}
	\UECEfig{}{
		\includegraphics[width=8cm]{figuras/figura-1}
	}{
		\Fonte{Elaborado pelo autor}
	}
\end{figure}
```

### Como inserir uma alínea
```tex
\begin{alineas}
	\item Lorem ipsum dolor sit amet;
    \item Praesent vitae nulla varius;
	\item Praesent quis erat eleifend;
	\item Mauris facilisis odio eu:
	\begin{subalineas}
		\item Integer non lacinia magna;
		\item Proin mattis placerat risus.
	\end{subalineas}
\end{alineas}
```

### Como criar Capítulos
```tex
\chapter{Fundamentação Teórica}
\label{cap:fundamentacao-teorica}
```

### Como criar Seções
```tex
% Seções Secundárias
\section{Objetivo Geral 2}
\label{sec:objetivo-geral-2}

% Seções Terciárias
\subsection{Objetivo Geral 3}
\label{sec:objetivo-geral-3}

% Seções Quaternárias
\subsubsection{Objetivo Geral 4}
\label{sec:objetivo-geral-4}

% Seções Quinárias
\subsubsubsection{Objetivo Geral 5}
\label{sec:objetivo-geral-5}
```

### Como inserir um algoritmo
```tex
\begin{algorithm}[h!]
	\SetSpacedAlgorithm
	\caption{\label{alg:algoritmo_de_colonica_de_formigas}Algoritmo de Otimização por Colônia de Formiga}
	\Entrada{Entrada do Algoritmo}
	\Saida{Saida do Algoritmo}
	\Inicio{
		Atribua os valores dos parâmetros\;
		Inicialize as trilhas de feromônios\;
		\Enqto{não atingir o critério de parada}{
			\Para{cada formiga}{
				Construa as Soluções\;
			}
			Aplique Busca Local (Opcional)\;
			Atualize o Feromônio\;
		}
	}
\end{algorithm}
```

# Atenção

O template é fornecido gratuitamente e sem garantias e pode ser redistribuído livremente para fins acadêmicos. Este é um produto extraoficial e não está oficialmente vinculado à Universidade Federal Rural de Pernambuco -- UFRPE.

# Agradecimentos

[Grupo de Otimização em Engenharia de Software -- GOES](http://www.goes.uece.br)

[Thiago Nascimento](https://github.com/thiagodnf)
