# Growing Neural Gas para Análise de Comportamento Educacional
Este projeto implementa e estende o algoritmo **Growing Neural Gas (GNG)** para análise não supervisionada do comportamento de alunos em listas de exercícios, utilizando métricas de desempenho e tempo.

## 📚 Contexto

O projeto foi desenvolvido no contexto de uma **pesquisa acadêmica**, utilizando dados reais de desempenho estudantil. O objetivo principal é compreender como os alunos evoluem ao longo do tempo, identificando padrões recorrentes e fluxos de transição entre diferentes estados de aprendizagem, sem o uso de rótulos.

---

## 🎯 Objetivos

- Aplicar o algoritmo **Growing Neural Gas** para clusterização adaptativa de dados educacionais  
- Modelar a evolução do comportamento dos alunos ao longo de múltiplas listas de exercícios  
- Analisar **transições temporais** entre estados de aprendizagem  
- Visualizar padrões utilizando **PCA** e **grafos direcionados**  
- Explorar aprendizado **não supervisionado** em um problema real

---

## 🧠 Metodologia

O pipeline do projeto segue as seguintes etapas:

1. **Seleção e pré-processamento dos dados**
   - Conversão de valores booleanos
   - Normalização com **Min-Max Scaling**

2. **Treinamento da Rede Growing Neural Gas**
   - Inicialização com poucos neurônios
   - Inserção dinâmica de neurônios com base no erro
   - Remoção de neurônios com baixo fator de utilidade
   - Atualização topológica entre neurônios

3. **Análise Temporal**
   - Registro das ativações dos neurônios ao longo do tempo
   - Modelagem das transições entre neurônios

4. **Visualização**
   - Redução de dimensionalidade com **PCA**
   - Visualização dos neurônios e dados projetados
   - Construção de grafos direcionados para análise de fluxo

---

## 🤖 Tipo de Aprendizado

Este projeto utiliza **Aprendizado Não Supervisionado**, uma vez que o modelo aprende padrões e estruturas nos dados sem o uso de rótulos ou classes pré-definidas.

O algoritmo Growing Neural Gas permite a adaptação dinâmica da topologia da rede conforme novos padrões são observados.

---

## 📊 Dados Utilizados

As métricas analisadas incluem, entre outras:

- Número de submissões
- Número de acertos
- Questões totalmente erradas
- Tempo total gasto
- Tempo médio por questão
- Número de questões por lista

Cada lista de exercícios é processada de forma incremental, permitindo a análise da evolução do comportamento dos alunos.

---

## 📈 Resultados

Os principais resultados obtidos incluem:

- Identificação de **padrões recorrentes de comportamento**
- Visualização clara da organização dos dados via PCA
- Modelagem do **fluxo de alunos** entre estados ao longo do tempo
- Representação gráfica das transições utilizando grafos direcionados

---

## 🛠️ Tecnologias Utilizadas

- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib**
- **NetworkX**

---
