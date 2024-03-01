# Etapas do Projeto

Este documento visa registrar as etapas necessárias à conclusão do projeto do *Ion Milling*. Os ítens aqui descritos são feitos em linhas gerais. Outros documentos contém a evolução do meu aprendizado nos conceitos envolvidos.

# Protocolo GPIB

Esta etapa envolve o uso de cabo GPIB, que é um protocolo de comunicação entre instrumentos laboratoriais e computadores. Ele permite a comunicação entre instrumentos também. Há uma pasta neste diretório dedicada a esse tema.

## Manuseio da Controladora de Fluxo de Massa

A *controladora de fluxo de massa* fará a ejeção de feixe de íons de argônio, o qual será ionizado pelo *gerador de plasma*, descrito no ítem seguinte. Controle computacional feito via cabo GPIB.

## Controle do Gerador de Plasma

O gerador de plasma fará a ionização do feixe de argônio, ejetado pela controladora de fluxo de massa. Seu controle será feito via cabo GPIB.

## Controle da Bomba de Vácuo

A bomba de vácuo fará o controle da rarefação da câmara por onde será transmitido o raio de íons de argônio. Aqui não deve haver impurezas, portanto a necessidade de vácuo. Controle via cabo GPIB.

## Interface Gráfica Com o Usuário

A interface gráfica com o usuário permitirá seleção de parâmetros ou mesmo conjuntos de parâmetros pré-estabelecidos de acordo com o tipo de amostra e arquitetura almejada. Eu sugeri um modelo $3D$ do canhão de plasma e da amostra para representar uma prévia do ângulo ajustado pelo usuário antes da execução do comando. Estou estudando a possibilidade de essa parte do projeto ser implementada com o Arduino, devido ao seu baixo custo, variedade de placas (*shields*) disponíveis e vasta documentação disponível. Contudo, ainda deve-se observar o quesito robustês do projeto ao se considerar o uso do Arduino. Um exemplo é a alta sensibilidade a cargas estáticas, o que pode comprometer seu uso aqui.
Uma possibilidade é introduzir um paradigma local, onde será possível controlar o equipamento diretamente via touchscreen, controlado via arduino, OU via computador pessoal, usando Pyvisa. Contudo, eu devo criar uma interface gráfica para o usuário que permitirá controlar os parâmetros do script feito em Pyvisa. Mais detalhes na pasta.

## Proteção contra cargas estáticas

Esta parte do projeto é muito importante de um ponto de vista geral, pois os microcontroladores envolvidos, *Arduino*, *Esp32* ou mesmo *Raspberry Pi* (ou os alternativos *Orange Pi* e *Banana Pi*) são sensíveis a cargas estáticas. Portanto, deve-se estudar aqui a criação de um sistema de proteção contra sobrecargas na alimentação e descarga de eletricidade estática nos microcontroladores.

## Proteção do usuário contra descargas elétricas

Deve-se implementar um módulo de proteção ao usuário contra descargas elétricas.