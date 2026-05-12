# GFT - Fundamentos de Cloud com AWS

Repositório criado para documentar o desafio prático do bootcamp **GFT - Fundamentos de Cloud com AWS** na DIO, aplicando os conhecimentos adquiridos nas aulas sobre gerenciamento de instâncias na AWS.

Além das práticas realizadas no laboratório, também foi feita a modelagem de um sistema de geração de boletos bancários utilizando serviços da AWS como exemplo de aplicação real.

---

## Descrição do desafio

O objetivo deste desafio foi consolidar os conhecimentos sobre infraestrutura em nuvem utilizando recursos da AWS.

Durante o laboratório foram abordados dois principais tópicos:

- Criação e uso de imagens AMI
- Criação de Snapshots EBS

Como complemento prático, foi modelado um sistema responsável pela geração de boletos, onde:

- Uma API hospedada em uma instância EC2 processa as requisições
- O armazenamento persistente utiliza volumes EBS
- Os boletos gerados são armazenados em um bucket do Amazon Simple Storage Service
- AMIs podem ser utilizadas para replicar rapidamente o ambiente
- Snapshots EBS podem ser usados para backup e recuperação

---

## Arquitetura modelada

Fluxo simplificado:

Cliente → API EC2 → Processamento de boletos → Armazenamento EBS → Upload para S3

### Evidência da arquitetura

![Arquitetura](images/arquitetura-boletos.png)


## Aprendizados

- Escalabilidade com AMI
- Backup com snapshots
- Armazenamento em S3
- Modelagem de arquitetura em nuvem
- Aplicação prática em sistema financeiro

---

## Conclusão

Este desafio ajudou a entender como serviços da AWS podem ser utilizados tanto em laboratórios técnicos quanto em cenários reais, como um sistema de geração de boletos.
