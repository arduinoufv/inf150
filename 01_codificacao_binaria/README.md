![](https://github.com/arduinoufv/inf150/blob/master/01_codificacao_binaria/FoYz1t8X0AAHCbx.jpeg?raw=true)

Sistemas de Numeração e Codificação: Binário, Complemento de 2, Hexadecimal, ASCII, Aritmética Binária. Codificação Esparsa e Compacta  

* [Laboratório](https://colab.research.google.com/drive/1U654FtCg5_ZEtmObc8SZIfZl4vk2pxDS) - Submeter pelo Google Classroom, usar sua conta @ufv. [Video com instruções](https://youtu.be/SmxgtQirgvs)

* [Video com Instruçoes para submissão do exercício](https://youtu.be/XcfEPMSZ1CU)

* [Video com instruções para questionário](https://youtu.be/bor-YXUZHNQ)


Python Code to generate the 8 bytes figure
```

import struct

x = b"computer"

print("8 8-bit integers:", struct.unpack("BBBBBBBB", x))
print("4 unsigned 16-bit integers:", struct.unpack("HHHH", x))
print("2 unsigned 32-bit integers:", struct.unpack("II", x))
print("1 unsigned 64-bit integer:", struct.unpack("Q", x))
print("a 64-bit pointer:", hex(struct.unpack("P", x)[0]))
print("6 ascii characters + 1 signed 16-bit integer:", struct.unpack("6sH", x))
print("2 32-bit floats:", struct.unpack("ff", x))
print("1 64-bit float:", struct.unpack("d", x))
print("2 RGB colors:", struct.unpack("BBBBBBBB", x))
```
