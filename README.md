# Sistema de Gerenciamento de Estacionamento

Projeto desenvolvido como solução para o desafio "Trilha .NET - Fundamentos" da Digital Innovation One (DIO). A aplicação consiste em um sistema de console construído em C# para realizar a gestão de veículos em um estacionamento, controlando entradas, saídas e cálculo de tarifação.

---

## Tabela de Conteúdos

- [Visão Geral](#visão-geral)
- [Funcionalidades](#funcionalidades)
- [Regra de Negócio](#regra-de-negócio)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Como Executar o Projeto](#como-executar-o-projeto)
- [Autor](#autor)

---

## Visão Geral

O objetivo principal do sistema é automatizar o fluxo básico de um estacionamento. O programa solicita valores tarifários iniciais e, através de um menu interativo no terminal, permite cadastrar placas, listar veículos estacionados e calcular o valor cobrado com base nas horas permanecidas.

---

## Funcionalidades

- **Configuração de Tarifas:** Definição do preço inicial e do preço por hora na inicialização da aplicação.
- **Cadastrar Veículo:** Entrada de placas de veículos para registro no sistema.
- **Listar Veículos:** Exibição de todos os veículos atualmente estacionados.
- **Remover Veículo:** Liberação de um veículo mediante verificação de placa, cálculo do valor total cobrado e remoção da lista.
- **Encerramento Seguro:** Opção para finalizar a execução do programa.

---

## Regra de Negócio

O cálculo do valor total a ser pago pelo condutor do veículo segue a seguinte fórmula:

$$\text{Valor Total} = \text{Preço Inicial} + (\text{Preço por Hora} \times \text{Horas Estacionado})$$

Caso não existam veículos cadastrados ao selecionar a opção de listagem ou remoção, o sistema exibe mensagens informativas ao usuário.

---

## Tecnologias Utilizadas

- **Linguagem:** C#
- **Plataforma:** .NET 8.0 (ou superior)
- **Tipo de Aplicação:** Console Application

---

## Estrutura do Projeto

```text
Estacionamento/
└── DesafioEstacionamento/
    ├── Models/
    │   └── Estacionamento.cs
    ├── Program.cs
    └── DesafioEstacionamento.csproj
