# Conceitos Estatísticos

## Desvios
A diferença entre os valores observados e a estimativa de localização.

**Sinônimos:** erros, resíduos

## Variância
A soma dos quadrados dos desvios da média, divididos por \( n - 1 \), em que \( n \) é o número de valores de dados. Em livros de estatística, existe sempre a discussão sobre por que temos \( n - 1 \), em vez de \( n \), no denominador da fórmula de variância, levando ao conceito de graus de liberdade. 

Essa distinção não é importante quando \( n \) é grande, pois não faz muita diferença se você divide por \( n \) ou \( n - 1 \). No entanto, se estiver interessado, o caso é o seguinte: Isso é baseado na premissa de que você quer fazer estimativas de uma população com base em uma amostra. Se utilizarmos o denominador intuitivo de \( n \) na fórmula de variância, subestimaremos o valor real da variância e o desvio-padrão da população. Isso se chama estimativa enviesada. No entanto, se dividirmos por \( n - 1 \), o desvio-padrão se torna uma estimativa não enviesada.

A explicação completa sobre por que o uso de \( n \) leva a uma estimativa enviesada envolve a noção de graus de liberdade, que considera o número de restrições no cálculo de uma estimativa. Nesse caso, existem \( n - 1 \) graus de liberdade, já que há uma restrição: o desvio-padrão depende do cálculo da média da amostra. Em muitos problemas, os cientistas de dados não precisam se preocupar com graus de liberdade, mas existem casos em que o conceito é importante.

**Sinônimo:** erro médio quadrático

## Desvio-padrão
A raiz quadrada da variância. O desvio-padrão é mais fácil de interpretar do que a variância, pois está na mesma escala que os dados originais. 

Embora sua fórmula seja mais complicada e menos intuitiva, o desvio-padrão é preferido na estatística em vez do desvio absoluto médio, devido à teoria estatística: matematicamente, trabalhar com valores quadráticos é mais conveniente do que com valores absolutos, especialmente em modelos estatísticos.

**Sinônimos:** norma \( l_2 \), norma Euclidiana

## Desvio Absoluto Médio
A média do valor absoluto dos desvios da média.

**Sinônimos:** norma \( l_1 \), norma Manhattan

## Desvio Absoluto Mediano da Mediana
A mediana do valor absoluto dos desvios da mediana. Nem a variância, nem o desvio-padrão, nem o desvio absoluto médio são robustos frente a outliers e valores extremos. 

A variância e o desvio-padrão são especialmente sensíveis aos outliers, pois são baseados em desvios quadráticos. Uma estimativa de variabilidade robusta é o desvio absoluto mediano da mediana (MAD).

## Amplitude
A diferença entre o maior e o menor valor no conjunto de dados.

## Estatísticas Ordinais
Métricas baseadas nos valores de dados classificados do menor ao maior.

**Sinônimo:** classificações

## Percentil
Valor tal que \( P \) por cento dos valores assumam esse valor ou menos, e \( (100 - P) \) por cento assumam esse valor ou mais.

**Sinônimo:** quantil

## Amplitude Interquartílica
A diferença entre o 75° percentil e o 25° percentil.

**Sinônimo:** IQR

---

## Ideias Chave
- A variância e o desvio-padrão são as estatísticas de variabilidade mais difundidas e comumente registradas.
- Ambos são sensíveis aos outliers.
- Métricas mais robustas incluem desvios absolutos (médio e mediano) e percentis (quantis).
