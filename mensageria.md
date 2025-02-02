# Mensageria
Mensageria é um conceito utilizado para comunicação assíncrona entre sistemas, onde mensagens são enviadas para filas e processadas posteriormente, garantindo maior eficiência e escalabilidade.

## Benefícios:
- **Processamento em background**: Em vez de processar as escritas imediatamente, as filas permitem o processamento em background.
- **Feedback instantaneo**: O usuário recebe um feedback instantâneo enquanto a fila processa a instrução, melhorando a experiência do usuário.

## Desafios:
- **Garantia de entrega**: Garantir que mensagens não sejam perdidas ou processadas mais de uma vez.
- **Escalabilidade e desempenho**: Lidar com altos volumes de mensagens e manter a performance.
- **Orquestração e monitoramento**: Controlar fluxos de mensagens e evitar gargalos na comunicação.

## Soluções de Mercado
- **Kafka**: Ideal para sistemas de alta escalabilidade e processamento em tempo real.
- **RabbitMQ**: Mensageria baseada no protocolo AMQP. Excelente para sistemas que exigem alta confiabilidade e roteamento de mensagens.
