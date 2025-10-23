# desafio-gerenciamento-ec2
# Desafio: Gerenciando Instâncias EC2 na AWS  

## Descrição do Projeto  
Este projeto faz parte do bootcamp da Digital Innovation One (DIO) e tem como objetivo consolidar os conhecimentos sobre gerenciamento de instâncias EC2 na AWS.  
Durante o desafio, foram aplicados conceitos práticos de criação, configuração e monitoramento de instâncias, reforçando o entendimento sobre a infraestrutura em nuvem da Amazon.  

---

## Objetivos de Aprendizagem  
- Aplicar os conceitos estudados sobre EC2.  
- Compreender o ciclo de vida de uma instância.  
- Documentar processos técnicos de forma organizada.  
- Utilizar o GitHub como ferramenta de portfólio técnico.  

---

## Etapas do Projeto  

### 1. Criação da Instância EC2  
- Serviço: Amazon EC2  
- Sistema Operacional: Amazon Linux 2  
- Tipo de Instância: t2.micro (elegível ao Free Tier)  
- Par de Chaves (Key Pair): criado para acesso via SSH  
- Grupo de Segurança:  
  - Porta 22 liberada (acesso SSH)  
  - Porta 80 liberada (acesso HTTP, se necessário)

O processo foi realizado pelo console da AWS, configurando corretamente a instância e ajustando as permissões de acesso no grupo de segurança.

---

### 2. Conexão com a Instância  
Com a instância em execução, a conexão foi feita via terminal utilizando o comando:

```bash
ssh -i "minha-chave.pem" ec2-user@ip-da-instancia
