# Biblia Ninja
Projeto para distribuição de arquivos da bíblia(csv e parquet) para uso em data science, NLP e outras aplicações visando partilhar iniciativas que contemplem o público de fala brasileira no aprofundamento bíblico. 

# Sistema VersoID(vId) - a id dos Versículos
Cada versículo é acessado por um id que é uma combinação dos números do livro+capitulo+versiculo.
vi isso pela primeira vez no https://github.com/scrollmapper/bible_databases

| Livro | Capítulo | Versículo |
| ----- | -------- | --------- |
|  00  |   001     | 000 |


Exemplo:

###  Genesis 1:1 (Genesis capítulo 1, versículo 1) = 01001001 ### (01 001 001)

Exodus 2:3 (Exôdo capítulo 2, versículo 3) = 02002003 (02 002 003)

O sistema vId pode ser usado como linguagem universal para tratamento de diversos outros arquivos de relação entre versículos, como referência cruzada, correspondencia de traduções ou associação de perícopes ou assuntos.

Trechos
01001001 - 05005005 pega  Gênesis 1:1 até Deuteronômio 5:5.

Referências Cruzadas
01001005 x 19074016 infere que Gênesis 1:5 tem relação com Salmos 74:16

# Linguagens e Versões
As linguagens e versões são específicadas nos nomes dos arquivos csv e parquet.

Exemplo:
pt_naa.csv - Português, Nova Versão Atualizada

Um arquivo com todas as abreviações de linguagens e versão é disponibilizado na pasta utils.
