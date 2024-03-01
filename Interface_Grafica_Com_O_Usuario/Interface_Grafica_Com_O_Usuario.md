Devemos criar uma interface gráfica com o usuário para o manuseiodo Ion Milling. Através dela, será feita a seleção de parâmetros individuais ou mesmo a seleção de programas, com parâmetros pré-estabelecidos. Ainda não foi decidido o formato da interface gráfica, mas eu já fiz algumas sugestões de funcionalidades a serem incluídas, como por exemplo um modelo 3D afim de mostrar o ângulo do canhão de plasma (se eu não me engano, era isso) de forma visual.

Como Clodoaldo sugeriu usarmos o Arduino para o controle da máquina, eu busquei alternativas envolvendo o Arduino também na interface gráfica com o usuário. (GUI).

O vídeo abaixo dá algumas dicas de como usar um touchscreen para criar uma interface gráfica usando Arduino. Ele inclui exemplos de projetos com seus códigos fonte no link da descrição.

[How to create a simple touchscreen GUI with Arduino ](https://www.youtube.com/watch?v=SIo_Gv7K7Fo)

O vídeo abaixo contém 3 exemplos bem legais usando interface gráfica via tela LCD TFT.

[Arduino TFT LCD Touch Screen Tutorial](https://www.youtube.com/watch?v=9Ms59ofSJIY)

## Comunicação local e remota com o Ion Milling.

O vídeo abaixo mostra me inspirou uma nova possibilidade:

[Lab Instrumento Automation with Python](https://www.youtube.com/watch?v=xko8wzEBqfc)

que é introduzir um paradigma misto, combinando o local, onde será possível controlar o equipamento diretamente via touchscreen, operado via Arduino ou ESP32, OU via computador pessoal, usando Pyvisa. Contudo, eu devo criar uma interface gráfica para o usuário que permitirá controlar os parâmetros do script feito em Pyvisa.

Uma maneira de fazer isso pode ser o uso de um shield de comunicação ethernet para o caso do Arduino ou diretamente via ESP32, o qual vai se comunicar com o computador pessoal munido do Software.








