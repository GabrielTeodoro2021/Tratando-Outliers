# Tratando-Outliers

Notebook usado para estudo a fim de tratar uma planilha excel de casas para alugar, onde após feita uma análise percebi que algumas casas tinham muito mais banheiros que outras, o que podia causar uma inconsistência na média de banheiros por casa.

Foi usado o IQR (Interquartile Range) é uma técnica estatística usada para identificar e tratar outliers (valores fora do padrão esperado) em um conjunto de dados. Ele ajuda a determinar a dispersão central dos dados, focando nos quartis (os percentis que dividem os dados em partes iguais).

Passos para calcular e usar o IQR para tratar outliers:
1. Organizar os dados
Primeiro, organize seus dados em ordem crescente (do menor para o maior valor).

2. Calcular os Quartis
Agora, calcule os quartis, que são os valores que dividem os dados em quatro partes iguais:

- Q1 (Primeiro Quartil): O valor no 25% da sequência de dados.
- Q2 (Mediana): O valor no 50% da sequência (meio dos dados).
- Q3 (Terceiro Quartil): O valor no 75% da sequência de dados.
  
3. Calcular o IQR
O IQR é a diferença entre o terceiro quartil (Q3) e o primeiro quartil (Q1): 
𝐼
𝑄
𝑅
=
𝑄
3
−
𝑄
1
IQR=Q3−Q1

4. Definir os Limites para Outliers
Agora, com o IQR calculado, você pode identificar os limites para considerar outliers:

Limite Inferior: 
𝑄
1
−
1
,
5
×
𝐼
𝑄
𝑅
Q1−1,5×IQR

Limite Superior: 
𝑄
3
+
1
,
5
×
𝐼
𝑄
𝑅
Q3+1,5×IQR

5. Identificar Outliers
Outliers inferiores: São os valores abaixo do limite inferior.
Outliers superiores: São os valores acima do limite superior.

6. Tratar Outliers
Existem diferentes formas de tratar os outliers:

 - Remover os outliers (simplesmente excluindo-os dos dados);
 - Substituir os outliers por um valor mais representativo (ex: a mediana ou a média);
 - Manter os outliers, se eles forem importantes para a análise.
