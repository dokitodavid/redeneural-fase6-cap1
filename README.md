# FIAP — Faculdade de Informática e Administração Paulista

<p align="center">
  <a href="https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP" width="40%"></a>
</p>

# FarmTech Solutions — Fase 6

## Visão Computacional e Redes Neurais

Equipe responsável pelas duas entregas obrigatórias da Fase 6.

## 👨‍🎓 Integrantes

| Integrante | RM |
|---|---|
| Renata de Almeida Marinho | 569342 |
| Pedro Henrique Lacerda | 573114 |
| Giselli Mayumi Takahashi Yokoyama | 572690 |
| João Otavio Moraes | 573227 |
| David Ribeiro Prado de Lacerda | 570350 |

## 👩‍🏫 Professores

### Tutora da Turma A

[Nicolly de Souza](https://github.com/nicollycrs).

### Coordenador(a)

André Godoi Chiovato.

## 📜 Descrição

A FarmTech Solutions está ampliando sua atuação em Inteligência Artificial e deseja demonstrar a aplicação prática de visão computacional. Este projeto utiliza imagens de gatos e tênis para estudar detecção de objetos e classificação de imagens.

A Entrega 1 customiza uma YOLOv5s para duas classes, com treinamentos de 30 e 60 épocas e um terceiro experimento com Early Stopping. Os modelos são comparados pelas métricas de validação e aplicados a oito imagens de teste, com análise visual das detecções e de suas limitações.

A Entrega 2 compara essa YOLOv5 customizada com uma YOLOv5 padrão e uma CNN treinada do zero. A avaliação considera facilidade de uso, desempenho, treinamento e inferência, respeitando a diferença entre detecção de objetos e classificação de imagens.

O dataset compartilhado possui 80 imagens: 32 por classe para treino, quatro para validação e quatro para teste. As imagens de treino e validação possuem rotulações no formato YOLO.

O desenvolvimento, o código, as saídas dos experimentos e as análises completas estão nos notebooks. Esta página apresenta a entrega e orienta o acesso aos seus arquivos.

### Entregáveis

| Entrega | Acesso |
|---|---|
| Entrega 1 — YOLOv5 customizada | [Abrir notebook](src/entrega_1/RenataDeAlmeidaMarinho_rm569342_PedroHenriqueLacerda_rm573114_GiselliMayumiTakahashiYokoyama_rm572690_JoaoOtavioMoraes_rm573227_DavidRibeiroPradoDeLacerda_rm570350_pbl_fase6.ipynb) |
| Entrega 2 — comparação entre YOLOv5 e CNN | [Abrir notebook](src/entrega_2/RenataDeAlmeidaMarinho_rm569342_PedroHenriqueLacerda_rm573114_GiselliMayumiTakahashiYokoyama_rm572690_JoaoOtavioMoraes_rm573227_DavidRibeiroPradoDeLacerda_rm570350_pbl_fase6.ipynb) |
| Dataset — imagens e rotulações | [Ver dataset.zip](dataset.zip) · [Baixar ZIP completo](https://media.githubusercontent.com/media/dokitodavid/redeneural-fase6-cap1/main/dataset.zip) |
| Vídeo demonstrativo da Entrega 1 | [Assistir no YouTube](https://youtu.be/j6Jf3tsRY2E) |
| Documento do projeto no modelo FIAP | [Ler relatório](document/ai_project_document_fiap.md) |

## 📁 Estrutura de pastas

```text
redeneural-fase6-cap1/
├── .github/
├── assets/
│   ├── logo-fiap.png
│   └── prints/entrega_1/
├── config/
├── dataset.zip
├── document/
│   ├── ai_project_document_fiap.md
│   └── other/
├── scripts/
├── src/
│   ├── entrega_1/
│   └── entrega_2/
├── .gitattributes
├── .gitignore
└── README.md
```

- **`.github/`**: orientação para registrar problemas do projeto.
- **`assets/`**: identidade visual da FIAP e prints dos experimentos.
- **`config/`**: descrição das configurações utilizadas pelos notebooks.
- **`dataset.zip`**: imagens e rotulações utilizadas nas duas entregas, organizado internamente em `dataset/train`, `dataset/val` e `dataset/test`.
- **`document/`**: relatório do projeto organizado conforme o modelo FIAP.
- **`scripts/`**: documentação sobre os scripts auxiliares; os experimentos desta entrega estão nos notebooks.
- **`src/`**: notebooks das Entregas 1 e 2, com código, saídas e análises.

## 🔧 Como executar o código

Os arquivos `.ipynb` são entregues no próprio repositório e podem ser abertos no Google Colab, ambiente utilizado nos experimentos.

1. Abra ou baixe o notebook escolhido e carregue-o no Google Colab.
2. Selecione um ambiente com GPU, se disponível. Os experimentos registrados utilizaram uma Tesla T4.
3. Execute as células na ordem apresentada. Elas configuram o ambiente, obtêm os dados e executam os experimentos.

**Cada notebook pode ser executado sozinho**, em uma nova sessão do Colab. O notebook da Entrega 2 executa a YOLOv5 padrão e a CNN e retoma os resultados registrados na Entrega 1 para a comparação.

O dataset é baixado automaticamente como `dataset.zip` da branch `main` de [redeneural-fase6-cap1](https://github.com/dokitodavid/redeneural-fase6-cap1). O carregamento verifica o SHA-256 do arquivo, extrai as pastas para `/content/dataset` e confere as quantidades de imagens por classe e a presença das rotulações antes dos experimentos. O repositório deve estar público e conter o ZIP publicado nessa branch.

O ZIP possui aproximadamente **214 MiB** e é armazenado com **Git LFS**. O download utilizado pelos notebooks fornece o conteúdo completo do arquivo, sem exigir a instalação do Git LFS no Colab. Para obter o dataset manualmente, use o link **Baixar ZIP completo** da tabela de entregáveis. Para clonar o repositório com o arquivo completo, utilize Git LFS no computador.

As células de preparação instalam as dependências da YOLOv5. A Entrega 2 também utiliza TensorFlow/Keras e scikit-learn disponíveis no ambiente Colab. As bibliotecas, configurações e versões registradas estão documentadas nos notebooks.

O armazenamento do Colab é temporário. Uma nova sessão requer a execução das etapas que carregam os dados e geram os modelos. Os caminhos `/content` e os comandos usados foram preparados para o Colab; executar em Jupyter local requer um ambiente compatível e adaptação desses caminhos.

**Disponibilização dos dados:** o uso do GitHub em substituição ao Google Drive foi autorizado para esta entrega. Os dois notebooks obtêm o ZIP diretamente do repositório, sem upload manual.

## 🗃 Histórico de lançamentos

- **13/10/2026 — versão inicial da entrega:** duas entregas organizadas no modelo FIAP, notebooks com resultados registrados, dataset em ZIP com Git LFS e documentação integrada ao vídeo demonstrativo.

## 📋 Licença

A apresentação e a estrutura documental foram adaptadas do **MODELO GIT FIAP**, atribuído à FIAP e disponibilizado sob [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/). Essa atribuição refere-se ao template e não declara uma licença adicional para as imagens do dataset.
