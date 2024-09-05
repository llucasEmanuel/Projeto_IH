# Infraestrutura de Hardware - Projeto RISC-V Pipeline 🚀

Este repositório contém o projeto da disciplina Infraestrutura de Hardware (IF674) no CIn-UFPE. O objetivo do projeto é implementar novas instruções em um processador RISC-V usando SystemVerilog.
---
Todos as instruções listadas foram implementas neste repositório pelos estudantes [Gabriel Alves](https://github.com/Gagdm), [Lucas Emanuel](https://github.com/llucasEmanuel) e [Mayres Andrey](https://github.com/mayresAndrey)
---

## 📝 Instruções

As instruções implementadas são as do conjunto RV32I, que é parte oficial do conjunto de instruções RISC-V. A tabela abaixo mostra o status de implementação das instruções no projeto atual:

| # | Instrução | Implementada | Testada | Funcionando |
|---|-----------|:-----------:|:-------:|:-----------:|
| 1 | `BEQ`     |     ✅     |   ✅   |     ✅     |
| 2 | `LW`      |     ✅     |   ✅   |     ✅     |
| 3 | `SW`      |     ✅     |   ✅   |     ✅     |
| 4 | `ADD`     |     ✅     |   ✅   |     ✅     |
| 5 | `AND`     |     ✅     |   ✅   |     ✅     |

Seu objetivo é implementar as instruções restantes listadas abaixo:

| # | Instrução | Implementada | Testada | Funcionando |
|---|-----------|:-----------:|:-------:|:-----------:|
| 1  | `JAL`     |      ✅     |    ✅    |      ✅      |
| 2  | `JALR`    |      ✅     |    ✅    |      ✅      |
| 3  | `BNE`     |      ✅     |    ✅    |      ✅      |
| 4  | `BLT`     |      ✅     |    ✅    |      ✅      |
| 5  | `BGE`     |      ✅     |    ✅    |      ✅      |
| 6  | `LB`      |      ✅     |    ✅    |      ✅      |
| 7  | `LH`      |      ✅     |    ✅    |      ✅      |
| 8  | `LBU`     |      ✅     |    ✅    |      ✅      |
| 9  | `SB`      |      ✅     |    ✅    |      ✅      |
| 10 | `SH`      |      ✅     |    ✅    |      ✅      |
| 11 | `SLTI`    |      ✅     |    ✅    |      ✅      |
| 12 | `ADDI`    |      ✅     |    ✅    |      ✅      |
| 13 | `SLLI`    |      ✅     |    ✅    |      ✅      |
| 14 | `SRLI`    |      ✅     |    ✅    |      ✅      |
| 15 | `SRAI`    |      ✅     |    ✅    |      ✅      |
| 16 | `SUB`     |      ✅     |    ✅    |      ✅      |
| 17 | `SLT`     |      ✅     |    ✅    |      ✅      |
| 18 | `XOR`     |      ✅     |    ✅    |      ✅      |
| 19 | `OR`      |      ✅     |    ✅    |      ✅      |
| 20 | `LUI`     |      ✅     |    ✅    |      ✅      |
| 21 | `HALT`    |      ✅     |    ✅    |      ✅      |

## 📁 Estrutura do repositório
O repositório está organizado da seguinte forma:
- [`design`](/design): Contém o código-fonte do projeto do processador RISC-V.
- [`doc`](/doc): Contém mais explicações sobre a implementação do pipeline.
- [`sim`](/sim): Contém exemplos de arquivos de simulação e seus resultados esperados.
- [`verif`](/verif): Contém os arquivos de testbench e as instruções de como testar o projeto.

## 📚 Recursos
- Para checar o conjunto de instruções RISC-V, consultar:
  - [Manual de Conjunto de Instruções RISC-V Volume I: ISA de Nível de Usuário - Documento Versão 2.2](https://riscv.org/wp-content/uploads/2017/05/riscv-spec-v2.2.pdf)
  - [risc-v isa pages, by msyksphinz](https://msyksphinz-self.github.io/riscv-isadoc/html/rvi.html#)

- Para simular e testar o projeto do processador RISC-V, utilizar:
  - [ModelSim-Intel® FPGAs Standard Edition Software Version 20.1.1](https://www.intel.com/content/www/us/en/software-kit/750666/modelsim-intel-fpgas-standard-edition-software-version-20-1-1.html)

- Para verificar os resultados:
  - Comparar resultados com os exemplos fornecidos em [`sim`](/sim)
  - Utilizar o simulador CompSim
  - Utilizar o [RISC-V Interpreter, by Cornell University](https://www.cs.cornell.edu/courses/cs3410/2019sp/riscv/interpreter/)
