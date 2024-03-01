# GPIB

GPIB parece ser um tipo de interface de dados. Devo aprender a usar isso de forma a controlar o acesso e transferência de dados via arduino.

[Fundamentals of GPIB](https://www.youtube.com/watch?v=MH-srU3bPmU&pp=ygUIR1BJQiB1c2I%3D)

[GPIB-to_USB interface with Arduino Nano UPDATE](https://www.youtube.com/watch?v=DAS1KVU_FaA)

## Controlando instrumentos GPIB via Python. 

No vídeo a seguir, [Remote GPIB control of instruments](https://www.youtube.com/watch?v=4bJGaGPRnbQ), partir dos $2:30$ minutos ele fala sobre um pacote chamado *Pyvisa*, que permite enviar comandos GPIB usando Python. Ele necessita de um adaptador, como o visto abaixo: 

<figure>
    <img src = "./images/Adaptador_GPIB_USB.png" alt="Adaptador GPIB/USB da National Instruments"
    width = "400"
    height = "200"
    style="display: block; margin: 0 auto"/>
    <figcaption> Adaptador GPIB/USB da National Instruments.</figcaption>
</figure>

Ele usa um driver proprietário encontrado na página [National Instruments GPB-USB-HS Driver](http://www.ni.com/en-ca/support/downloads/drivers/downloads.ni-488-2.html#305442).

Retomando ao vídeo, aos $5:31$ minutos, o autor mostra como obter o endereço GPIB de alguns instrumentos de medida, como um *Controlador de Polarização* e um *Atenuador Ótico*.

<figure>
    <img src = "./images/Enderecos_GPIB_Via_PYVISA.png" alt="Saída de endereços GPIB de instrumentos, via Pyvisa."
    width = "400"
    height = "100"
    style="display: block; margin: 0 auto"/>
    <figcaption> Biblioteca Python Pyvisa acessando endereços GPIB de instrumentos de laboratório. A saída do programa foi destacada no quadrado azul, à direita.</figcaption>
</figure>

O vídeo sugere também olhar o manual de instruções dos instrumentos para verificar os comandos computacionais que podem ser emitidos via GPIB.

Eu parei aos $8:24$ no vídeo.