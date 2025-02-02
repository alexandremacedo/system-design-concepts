# Caching
O caching é uma técnica essencial em sistemas de alta performance, especialmente em cenários com grande volume de leituras ou dados que mudam raramente (low churn data). Sua implementação reduz a carga no banco de dados e melhora significativamente os tempos de resposta.

## Benefícios
- Redução do tempo de acesso a dados.
- Diminuição da carga em recursos de backend.
- Aumento da escalabilidade do sistema.

## Desafios
- Manter o cache sincronizado com o banco de dados
- Lidar com a expiração do cache: Dados armazenados podem expirar, levando a possíveis problemas de stale data (dados desatualizados).

## Estratégias para Consistência de Cache
- TTL (Time-to-Live) nas Keys:
  - Define um tempo de validade para cada item armazenado no cache.
  - Após o tempo expirar, o dado é removido automaticamente, garantindo que apenas informações recentes sejam acessadas.
- Write-through Caching:
  - Toda escrita no banco de dados é imediatamente refletida no cache.
  - Garante que os dados mais recentes estejam sempre disponíveis no cache.

## Soluções de Mercado
Duas das mais populares são:
- Memcached
- Redis
