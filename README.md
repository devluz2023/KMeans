# 📊 Custom KMeans Clustering Engine - Machine Learning from Scratch (Java)

Este repositório contém a implementação nativa e do zero (*from scratch*) do algoritmo de agrupamento **K-Means**, desenvolvida inteiramente na linguagem **Java**. O objetivo deste projeto é demonstrar o domínio conceitual, matemático e estrutural do aprendizado de máquina não supervisionado (*Unsupervised Learning*), sem a dependência de bibliotecas ou frameworks externos de Machine Learning.

---

## 🏗️ Estrutura e Organização do Projeto

O código segue a convenção clássica de pacotes para isolamento de escopo no desenvolvimento Java:

* **`src/br/com/kmean/main/`:** Diretório que centraliza o código-fonte (`.java`). Contém as classes que implementam a lógica do algoritmo, como a definição de pontos no espaço vetorial, cálculo de centroides, atribuição de clusters, além do ponto de entrada (`main`) para execução dos testes de agrupamento.
* **`bin/br/com/kmean/main/`:** Pasta que armazena os bytecodes compilados (`.class`) prontos para execução pela Java Virtual Machine (JVM).
* **`.DS_Store`:** Arquivo temporário de indexação de sistema de arquivos, devidamente isolado no controle de versão.

---

## 🧮 Funcionamento Matemático Implementado

O algoritmo foi codificado respeitando o fluxo iterativo tradicional do modelo K-Means:

1. **Inicialização:** Definição do número de agrupamentos ($K$) e posicionamento inicial dos centroides no espaço multidimensional.
2. **Cálculo de Distância:** Mensuração da proximidade geométrica entre cada ponto de dado e os centroides utilizando a métrica de **Distância Euclidiana**:
   $$d(p, q) = \sqrt{\sum_{i=1}^{n} (q_i - p_i)^2}$$
3. **Atribuição de Clusters:** Associação de cada ponto de dado ao centroide mais próximo.
4. **Atualização dos Centroides:** Recálculo da posição de cada centroide através da média aritmética das coordenadas de todos os pontos atribuídos a ele.
5. **Critério de Parada:** Repetição contínua dos passos 2, 3 e 4 até que os centroides estabilizem (convergência) ou o limite máximo de iterações configurado seja atingido.

---

## 🛠️ Stack Tecnológica

* **Linguagem Core:** Java (Strongly Typed & Object-Oriented).
* **Ambiente de Execução:** Java Virtual Machine (JVM) / JDK Core.
* **Paradigma de Programação:** Orientação a Objetos Avançada (Abstração de Vetores, Pontos e Centroides).

---

## 🎯 Relevância Estratégica no Perfil de Engenharia de IA

Escrever algoritmos de Machine Learning nativamente em Java confere diferenciais competitivos fundamentais para cenários de Big Data e MLOps:

1. **Entendimento Algorítmico Profundo:** Prova que você compreende como os pesos e as distâncias funcionam por baixo do capô, permitindo depurar e otimizar hiperparâmetros de modelos de mercado com muito mais propriedade.
2. **Computação de Alta Performance:** Java oferece excelente gerenciamento de memória e velocidade de execução. Implementar o K-Means diretamente na JVM permite que o modelo seja acoplado de forma nativa e extremamente veloz em sistemas core e esteiras de dados de baixa latência.
