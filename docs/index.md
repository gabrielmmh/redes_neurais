# Relatórios de Atividades — Redes Neurais (2025.1)

???+ info inline end "Última atualização"
    **16/11/2025**

## Aluno
- Gabriel Mendonça de Mello Hermida

---

## Atividades (notebooks)

- [x] **Atividade 1 — Pré-processamento (Spaceship Titanic)**

  _Notebook:_ [`exercises/01_data/data.ipynb`](./exercises/01_data/data.ipynb)

  Análise exploratória do dataset Spaceship Titanic com foco na variável *Transported*. Identificação de ausências (~2% em várias colunas) e tratamento por imputação (mediana para numéricos, moda para categóricos). Variáveis de gasto receberam transformação log1p seguida de padronização para reduzir caudas longas. Histogramas comparativos demonstram a normalização obtida.

- [x] **Atividade 2 — Perceptron *from scratch***

  _Notebook:_ [`exercises/02_perceptron/perceptron.ipynb`](./exercises/02_perceptron/perceptron.ipynb)

  Implementação de perceptron para dois cenários. No cenário separável, o modelo converge em poucas épocas com acurácia 100%. No cenário não separável, a sobreposição entre classes causa oscilações de acurácia (50-70%) e ausência de convergência, demonstrando a limitação do modelo para fronteiras não lineares.

- [x] **Atividade 3 — MLP *from scratch***

  _Notebook:_ [`exercises/03_mlp/mlp.ipynb`](./exercises/03_mlp/mlp.ipynb)

  Implementação de MLPs para classificação binária e multiclasse. No caso binário, acurácia de 62%. No multiclasse, MLP raso atinge 72.3% enquanto MLP com duas camadas ocultas atinge 80.7%, evidenciando o ganho de capacidade com maior profundidade.

- [x] **Atividade 4 — Variational Autoencoders (VAE)**

  _Notebook:_ [`exercises/04_vae/vae.ipynb`](./exercises/04_vae/vae.ipynb)

  VAE implementado para MNIST com 652k parâmetros. Utiliza reparameterization trick e beta annealing (β: 0→1 em 10 épocas). Loss final: 102.64 (BCE: 76.81, KL: 25.82). Visualizações incluem reconstrução, geração amostral e espaço latente via t-SNE.

---

## Projetos

- [x] **Projeto 1 — Classificação (MABe Mouse Behavior)**

  _Link:_ [caioboa.github.io/.../model](https://caioboa.github.io/DeepLearningPages/classification/model)

  **Autores:** Caio Boa, Gabriel Hermida e Pedro Civita

  Classificação de comportamentos de camundongos usando dataset CalMS21. O modelo identifica padrões de movimento a partir de dados de rastreamento.

- [x] **Projeto 2 — Regressão (Bike Sharing Demand)**

  _Link:_ [pedrocivita.github.io/projects/2](https://pedrocivita.github.io/projects/2/)

  **Autores:** Caio Boa, Gabriel Hermida e Pedro Civita

  Previsão de demanda de bicicletas compartilhadas usando MLP. O modelo utiliza variáveis climáticas e temporais, alcançando R²=0.88 e RMSE=63.44.

- [x] **Projeto 3 — Modelos Generativos (Stable Diffusion + ControlNet)**

  _Notebook:_ [`projects/generative/generative.ipynb`](./projects/generative/generative.ipynb)

  **Autores:** Caio Boa, Gabriel Hermida e Pedro Civita

  Geração de imagens de produtos usando Stable Diffusion 1.5 com ControlNet Canny para controle espacial. Pipeline inclui 5 exemplos com variação de hiperparâmetros e análise comparativa.

