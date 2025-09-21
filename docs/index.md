# Relatórios de Atividades — Redes Neurais (2025.1)

???+ info inline end "Última atualização"
    **21/09/2025**

## Aluno
- Gabriel Mendonça de Mello Hermida

---

## Atividades (notebooks)

- [x] **Atividade 1 — Pré-processamento (Spaceship Titanic)**  
  _Notebook:_ [`exercises/01_data/data.ipynb`](./exercises/01_data/data.ipynb)  
  **O que foi feito:** descrição do objetivo (*Transported*), identificação de variáveis numéricas e categóricas, auditoria de ausências (~2% em várias colunas).  
  **Pré-processamento:** imputação (mediana p/ numéricos; mais frequente p/ categóricos), one-hot encoding, padronização; para gastos (`RoomService`, `FoodCourt`, `ShoppingMall`, `Spa`, `VRDeck`) aplicou-se **log1p + padronização** para reduzir caudas longas.  
  **Evidências:** histogramas “antes/depois” de `Age` (padronizada) e `FoodCourt` (log1p + padronizada), mostrando centralização e escala adequadas à `tanh`.

- [x] **Atividade 2 — Perceptron *from scratch***  
  _Notebook:_ [`exercises/02_perceptron/perceptron.ipynb`](./exercises/02_perceptron/perceptron.ipynb)  
  **Cenário A (separável):** médias bem separadas e baixa variância → **convergência em poucas épocas** e **acurácia 100%**; fronteira linear sem erros residuais.  
  **Cenário B (não separável):** médias próximas e maior variância → **sobreposição**, oscilações de acurácia (~50–70%) e **não convergência**, evidenciando a limitação do perceptron para fronteiras não lineares.

- [x] **Atividade 3 — MLP *from scratch***  
  _Notebook:_ [`exercises/03_mlp/mlp.ipynb`](./exercises/03_mlp/mlp.ipynb)  
  **Binário (2D, 1 oculta):** MLP raso (tanh → sigmoid, BCE). Perda estabiliza ~0.52; **acurácia de teste ~62%**; fronteira separa parcialmente com erros em zonas de sobreposição.  
  **Multiclasse (3 classes):**  
  • MLP raso: perda final ~0.68; **acurácia de teste 72,3%**.  
  • MLP profundo (2 ocultas): perda final ~0.47; **acurácia de teste 80,7%**.  
  **Conclusão:** aumentar profundidade melhora a capacidade de representação e o desempenho.

---

## Próximos passos
- [ ] **Atividade 4 — Métricas** (organizar notebook em `exercises/04_metrics/` com avaliação padronizada: matriz de confusão, curvas ROC/PR e métricas por classe)
