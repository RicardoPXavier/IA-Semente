# Sistema Inteligente de Classificação de Sementes de Soja

## Resumo do Sistema

Este notebook implementa um sistema completo de classificação inteligente para sementes de soja, atendendo a todos os requisitos especificados:

###  Requisitos Implementados

#### Métodos de Extração de Características
- **GLCM (Gray-Level Co-occurrence Matrix)**: Extrai características de textura baseadas em co-ocorrência
- **LBP (Local Binary Pattern)**: Analisa padrões locais de textura
- **LPQ (Local Phase Quantization)**: Características baseadas em fase local
- **Características Combinadas**: Fusão de GLCM + LBP + LPQ para maior poder discriminativo

#### Classificadores Implementados
- **k-NN (k-Nearest Neighbors)**: Classificação baseada em proximidade
- **SVM (Support Vector Machine)**: Separação por hiperplanos ótimos
- **Árvore de Decisão**: Regras de decisão hierárquicas
- **MLP (Multi-Layer Perceptron)**: Rede neural artificial
- **Random Forest**: Ensemble de árvores de decisão

#### Otimização de Hiperparâmetros
- **GridSearchCV** com validação cruzada para cada classificador
- Busca exaustiva nos melhores parâmetros para maximizar F1-Score
- Normalização automática dos dados com StandardScaler

#### Avaliação Rigorosa
- **Validação Cruzada Estratificada** (k=5 folds)
- **Métricas Completas**: Acurácia, F1-Score, Precision, Recall
- **Matriz de Confusão** (5×5) para análise detalhada de erros
- **Relatórios Comparativos** entre todas as configurações

### Classes de Sementes
1. **Broken soybeans** (Sementes quebradas)
2. **Immature soybeans** (Sementes imaturas) 
3. **Intact soybeans** (Sementes íntegras)
4. **Skin-damaged soybeans** (Sementes com danos na pele)
5. **Spotted soybeans** (Sementes manchadas)

### Como Usar o Sistema

1. **Execute todas as células em ordem** para treinar e avaliar os modelos
2. **Compare os resultados** entre diferentes extratores e classificadores
3. **Analise as matrizes de confusão** para entender padrões de erro
4. **Utilize o melhor modelo salvo** para futuras classificações

### Outputs Esperados
- Tabelas comparativas de desempenho
- Gráficos de visualização de resultados
- Matriz de confusão detalhada
- Modelo otimizado salvo em arquivo
- Relatório final completo

### Tecnologias Utilizadas
- **scikit-learn**: Algoritmos de ML e métricas
- **skimage**: Processamento de imagens e extração de características
- **numpy/pandas**: Manipulação de dados
- **matplotlib/seaborn**: Visualizações
- **scipy**: Funções matemáticas avançadas

---

**Dica: Para obter os melhores resultados, execute todas as células em sequência. O sistema automatically escolherá a melhor configuração baseada no F1-Score.

Desenvolvido por
Ricardo de Paula Xavier
Matheus Floriano Saito
João Victor Bonilha

**Codigo Base foi disponibilizado pelo professor da disciplina**
