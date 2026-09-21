# 🏨 Sistema de Hospedagem

Projeto desenvolvido durante a **Trilha .NET — Explorando a Linguagem C#**, da [DIO](https://www.dio.me/).

O projeto consiste em um sistema de hospedagem desenvolvido em **C#**, utilizando conceitos fundamentais da linguagem e de Programação Orientada a Objetos (POO).

## 📋 Sobre o projeto

O sistema permite realizar reservas em um hotel, relacionando:

* **Pessoa** — representa os hóspedes;
* **Suíte** — representa a acomodação disponível;
* **Reserva** — relaciona os hóspedes e a suíte, além de realizar os cálculos da hospedagem.

O projeto foi desenvolvido a partir de uma estrutura inicial disponibilizada no desafio, sendo implementadas as regras e validações solicitadas.

## ⚙️ Funcionalidades

O sistema possui as seguintes funcionalidades:

* Cadastro de hóspedes em uma reserva;
* Cadastro da suíte;
* Consulta da quantidade de hóspedes;
* Cálculo do valor total da hospedagem;
* Aplicação automática de **10% de desconto para reservas de 10 dias ou mais**;
* Validação da capacidade da suíte;
* Exceção quando a quantidade de hóspedes ultrapassa a capacidade da suíte.

## 📌 Regras implementadas

### 1. Validação da capacidade da suíte

Não é possível cadastrar uma quantidade de hóspedes superior à capacidade da suíte.

Exemplo:

```text
Capacidade da suíte: 2 pessoas
Hóspedes: 3 pessoas

Resultado: Exception
```

### 2. Quantidade de hóspedes

O método `ObterQuantidadeHospedes()` retorna a quantidade total de hóspedes cadastrados na reserva.

### 3. Cálculo da hospedagem

O valor é calculado utilizando:

```text
Dias reservados × Valor da diária
```

### 4. Desconto

Para reservas de **10 dias ou mais**, é aplicado um desconto de **10%** sobre o valor total da hospedagem.

Exemplo:

```text
10 dias × R$ 100,00 = R$ 1.000,00

Desconto de 10% = R$ 100,00

Valor final = R$ 900,00
```

## 🛠️ Tecnologias utilizadas

* C#
* .NET
* Programação Orientada a Objetos
* Git
* GitHub

## 📂 Estrutura do projeto

```text
Sistema-de-Hospedagem/
│
├── Models/
│   ├── Pessoa.cs
│   ├── Reserva.cs
│   └── Suite.cs
│
├── Program.cs
├── diagrama_classe_hotel.png
└── README.md
```

## ▶️ Como executar

### Pré-requisitos

É necessário ter o **.NET SDK** instalado.

Verifique a instalação com:

```bash
dotnet --version
```

### Executando o projeto

Clone o repositório:

```bash
git clone https://github.com/mariayasmim2904-alt/Sistema-de-Hospedagem.git
```

Entre na pasta:

```bash
cd trilha-net-explorando-desafio
```

Execute o projeto:

```bash
dotnet run
```

Para verificar se o projeto compila corretamente:

```bash
dotnet build
```

## 📚 Aprendizados

Durante o desenvolvimento deste projeto, foram praticados conceitos importantes de C#, como:

* Classes e objetos;
* Propriedades;
* Métodos;
* Construtores;
* Listas;
* Estruturas condicionais;
* Exceções;
* Encapsulamento;
* Relacionamento entre classes;
* Programação Orientada a Objetos.

## 🎯 Objetivo

Este projeto faz parte da minha jornada de estudos em **C# e .NET**, com o objetivo de praticar os fundamentos da linguagem e desenvolver projetos para compor meu portfólio.

---

### 📖 Referência

Desafio proposto pela **DIO — Digital Innovation One**, na Trilha .NET — Explorando a Linguagem C#.

🌐 [DIO](https://www.dio.me/)
