# Resolução CONAMA 357-05

<br>

Por meio da [Resolução CONAMA 357](https://www.icmbio.gov.br/cepsul/images/stories/legislacao/Resolucao/2005/res_conama_357_2005_classificacao_corpos_agua_rtfcda_altrd_res_393_2007_397_2008_410_2009_430_2011.pdf), de 17.03.2005, que *"dispõe sobre a classificação dos corpos de água e diretrizes ambientais para o seu enquadramento, bem como estabelece as condições e padrões de lançamento de efluentes, e dá outras providências"*, são apresentados os padrões de qualidade de águas interiores.

A Resolução sofreu algumas alterações, por exemplo pela Resolução CONAMA 430, que revogou o artigo 24, que trata de lançamento de efluentes em curso d´água (corpo receptor).

<br>

**Padrão de Qualidade**

- Artigo X: Curso d'água de Classe X

----

### Objetivo

O projeto objetiva disponibilizar os parâmetros de qualidade em formato tabular, adequado para utilização em análises computacionais.

<br>

----

### Como Instalar?

<br>

```bash
pip install conama-357 --upgrade
```

<br>

----

### Como Usar?

<br>

```python
from normas import conama_357

# Get Table
df_357, list_classes = conama_357.get_parameters()

# Filter Data by "Classe"
df_357, list_parametrs = conama_357.filter_by_classe(df_357, classe='Classe 2')

# Filter Data by "Parâmetro"
dict_357 = filter_by_parameters(df_357, parametro='Oxigênio Dissolvido')
print(dict_357)
```

<br>

-----

### *TODO*

1. <strike>Compilar: Padrão de Qualidade para Classe 1, em Águas Doces (Artigo 14)</strike>
2. <strike>Compilar: Padrão de Qualidade para Classe 2, em Águas Doces (Artigo 15)</strike>
3. <strike>Compilar: Padrão de Qualidade para Classe 3, em Águas Doces (Artigo 16)</strike>
4. <strike>Compilar: Padrão de Qualidade para Classe 4, em Águas Doces (Artigo 17)</strike>
5. <strike>Compilar: Padrão de Lançamento (Artigo 34)</strike>
6. *Scripts*
7. Desenvolver *setup*
8. Compilar: Padrão de Qualidade para Classe 1, em Águas Doces onde ocorre pesca ou cultivo de organismo para fins de consumo intensivo (Artigo 14)
9. Compilar: Padrão de Qualidade para Classe 1, em Águas Salinas (Artigo 18)
10. Compilar: Padrão de Qualidade para Classe 2, em Águas Salinas (Artigo 19)
11. Compilar: Padrão de Qualidade para Classe 3, em Águas Salinas (Artigo 20)
12. Compilar: Padrão de Qualidade para Classe 1, em Águas Salobras (Artigo 21)
13. Compilar: Padrão de Qualidade para Classe 2, em Águas Salobras (Artigo 22)
14. Compilar: Padrão de Qualidade para Classe 3, em Águas Salobras (Artigo 23)

