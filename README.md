# HELP do Simulador

## Características da CPU

O simulador implementa uma CPU educacional baseada em uma arquitetura simplificada, voltada ao ensino de Arquitetura e Organização de Computadores. As principais características são:

- Conjunto de **12 instruções**, todas codificadas em **16 bits**
- **Memória de Dados** com capacidade para **256 palavras**
- **Memória de Instruções** com capacidade para **256 palavras**
- **8 registradores de uso geral** (R0 a R7)
- Suporte aos modos de execução **Monociclo** e **Multiciclo**

---

## Instruções Assembly

O simulador utiliza uma linguagem Assembly própria, definida especificamente para esta arquitetura.

- Cada instrução possui uma **descrição breve**, apresentada em uma única linha
- As variáveis devem ser declaradas utilizando **valores inteiros em formato decimal**
- O uso de **labels** é permitido para identificação de endereços no código:
  - Devem iniciar com **letras**
  - Podem conter **números**, desde que não sejam o primeiro caractere
  - Não são permitidos caracteres especiais ou espaços

---

## Formato das Instruções (ISA)

As instruções seguem os formatos definidos pela **ISA (Instruction Set Architecture)** do simulador.  
Cada formato especifica a posição dos campos como **opcode**, registradores e valores imediatos.

Os formatos são apresentados por meio de **figuras**, facilitando a visualização da organização dos 16 bits e o entendimento do processo de decodificação das instruções.

---

## Sinais de Controle

O simulador disponibiliza os sinais de controle utilizados durante a execução das instruções, permitindo uma análise detalhada do funcionamento interno da CPU.

- Cada sinal possui uma **descrição breve**, indicando seu significado e valores possíveis
- Os sinais são apresentados separadamente para:
  - **Versão Monociclo**, na qual todos os sinais são ativados em um único ciclo
  - **Versão Multiciclo**, na qual os sinais variam conforme o estado atual da máquina de controle

---

## Operação do Simulador

A interação com o simulador é realizada por meio dos seguintes controles:

- **ASSEMBLE (Montar)**: traduz o código Assembly para a representação interna de instruções
- **PLAY**: inicia a execução contínua do programa
- **PAUSE**: pausa a execução no ciclo atual
- **STOP**: encerra a execução e reinicia o estado do simulador
- **FORWARD (Passo-a-Passo)**: executa o programa de forma controlada, permitindo análise instrução por instrução ou ciclo a ciclo

---

## Configurações do Simulador

O simulador permite ajustar diferentes opções de execução e visualização:

- Exibição de valores em **Hexadecimal** ou **Decimal**
- Operação **Com Sinal** ou **Sem Sinal**, influenciando a interpretação dos dados
- Seleção do modo de execução **Monociclo** ou **Multiciclo**

Essas configurações auxiliam na análise do comportamento da CPU sob diferentes perspectivas.

---

## Contato e Sugestões

Sugestões, relatos de erros e contribuições podem ser enviados por meio do **repositório GitHub do projeto**.  
As mensagens enviadas pelo sistema de issues ou contato do Git são encaminhadas para os e-mails dos desenvolvedores responsáveis.
