# Configurações do projeto

A configuração do dataset da YOLOv5 é gerada pelo notebook da Entrega 1. Ela utiliza duas classes: `0` para gato e `1` para tênis, com caminhos de treino e validação em `/content/dataset`.

Os experimentos da YOLOv5 utilizam imagens de entrada de 640 pixels, batch size 16 e pesos iniciais `yolov5s.pt`. Os treinamentos de referência têm 30 e 60 épocas; o terceiro define até 90 épocas com paciência de 10 para Early Stopping.

A CNN da Entrega 2 utiliza entrada de 224 × 224 pixels, batch size 16, otimizador Adam, perda binary cross-entropy e Early Stopping monitorando `val_loss`, com paciência de cinco épocas.

As configurações executáveis e as justificativas estão nos [notebooks](../src/README.md).
