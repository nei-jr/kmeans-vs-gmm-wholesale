# K-means vs GMM do zero em PyTorch

Comparação entre K-means e Gaussian Mixture Model (via algoritmo EM),
implementados sem sklearn, no dataset Wholesale Customers (UCI).

## O que foi feito
- Remoção de outliers por distância de Mahalanobis (corte χ² a 97,5%)
- K-means e GMM implementados manualmente
- Validação com o rótulo real (canal: Horeca vs Varejo)
- Visualização dos clusters via PCA

## Resultados
| Modelo  | Concordância com o canal |
|---------|--------------------------|
| K-means | ~88%                     |
| GMM     | ~79%                     |

## Próximos passos
- Transformação log para reduzir a assimetria
- Avaliação com Adjusted Rand Index (ARI)

## Dados
[Wholesale Customers – UCI](https://archive.ics.uci.edu/dataset/292/wholesale+customers)
