# Projeto_FonteDeTensaoAjustavel
## Descrição:
Projeto da disciplina SSC0180 - Eletrônica para Computação, ministrada pelo professor Eduardo do Valle Simoes, com o objetivo de projetar uma
fonte reficadora capaz de transformar corrente alternada de tensão, em corrente contínua, com valor de tensão ajustável entre 3 e 12 volts.


## Componentes:

| Componente             |  Quantidade   | Especificações    | Valor Unitário |
|:----------------------:|:-------------:|:-----------------:|:--------------:|
| Diodo Retificador      | 5             | 1N4007 LGE=1N4004 | R$ 0,20        |
| Capacitor              | 1             | 680UFX25V         | R$ 5,80        |
| LED                    | 2             | 5mm VM difuso     | R$ 0,50        |
| Resistor               | 5             | CR25 3K3          | R$ 0,07        |
| Resistor               | 5             | CR25 1K           | R$ 0,07        |
| Resistor               | 5             | CR25 4K7          | R$ 0,07        |
| Resistor               | 5             | CR25 120R         | R$ 0,07        |
| Resistor               | 5             | CR25 680R         | R$ 0,07        |
| Diodo Zener            | 2             | 13V 1W - 1N4743   | R$ 0,50        |
| Potenciômetro          | 2             | 1W B10K B-16      | R$ 7,00        |
| Transistor             | 1             | BC368 N-25V-1A-0  | R$ 0.44        |
| Jumper Macho           | 10            | 20cm              | R$ 0,70        |
| Fusível                | 2             | 20 AG 0.1A        | R$ 1,10        |
| Varistor               | 1             | 150VAC 7D 241K    | R$ 1,50        |
|**Total**               |               |                   | **R$ 35,69**   |



## Sobre os componentes
#### Transformador:
A fonte de corrente alternada (tomada) fornece uma ddp de 127V, por isso é necessário o uso do transformador que é capaz de baixar a tensão de 110 volts para 12 volts.

#### Fusível:
O fusível é usado com o intuito de "proteger" o circuito de correntes elétricas excessivas, visto que se houver sobrecarga, ele irá interromper o circuito.

#### Ponte de diodos:
Formada por quatro diodos retificadores, é responsável por permitir que uma corrente alternada seja convertida em corrente contínua.

#### Varistor:
Também usado para maior segurança ao circuito, pois quando uma tensão excessiva é aplicada ao varistor, sua resistência diminui rapidamente, permitindo que ele conduza a corrente elétrica e desvie a energia extra para a terra ou para a fonte de alimentação.

#### Capacitor:
Responsável por controlar a ondulação da tensão no circuito, durante a alternância dos ciclos de corrente elétrica, o capacitor armazena energia (quando a tensão está alta) e libera quando a tensão cai.

#### Resistor:
O resistor limita o fluxo de corrente elétrica em um circuito, impedindo que a corrente ultrapasse o limite estabelecido por cada componente.

#### Diodo Zener:
Se comporta como um diodo normal, porém quando a tensão excede a tensão Zener, ele deixará "passar" somente a tensão limite, que no caso será 12V.

#### Transistor:
O transistor tem capacidade de controle da intensidade da corrente elétrica que passa por ele, sendo capaz de limitá-la, amplificá-la ou, até mesmo, atenuá-la.

#### Potenciômetro:
É um tipo de resistor que permite controlar a tensão entre 3 a 12V, no nosso caso.



## Foto do circuito na protoboard

![f5c56527-f483-4b29-b497-7117711fcc6f](https://github.com/GabriellaAlmeida07/Projeto_FonteDeTensaoAjustavel/assets/135055000/586c00af-1137-4ef8-8135-badcd054a8c8)

![b0ad6359-cd21-43d9-9d8b-161e95a4ce8e](https://github.com/GabriellaAlmeida07/Projeto_FonteDeTensaoAjustavel/assets/135055000/00809375-4016-438e-a1ba-d3aabf90693f)


## Circuito Falstad
[Circuito Falstad](https://tinyurl.com/2bdvvonj)
![circuito](https://github.com/GabriellaAlmeida07/Projeto_FonteDeTensaoAjustavel/assets/135055000/d42b11c0-0516-4a29-bf5d-487cf6339651)




## Projeto do Esquemático EAGLE

![Captura de tela 2024-06-18 152255](https://github.com/GabriellaAlmeida07/Projeto_FonteDeTensaoAjustavel/assets/135055000/972a8a0c-1e4a-4238-b6b5-66bf73dc3e55)




## Projeto PCB EAGLE
![Captura de tela 2024-06-18 151144](https://github.com/GabriellaAlmeida07/Projeto_FonteDeTensaoAjustavel/assets/135055000/2245b80e-6732-4328-9988-64db65348ff2)



## Cálculos
Queremos um Ripple pequeno (10%), e por isso é possível utilizar a fórmula simplificada C = i / (f * v) * ripple.

Seguindo o simulador Falstad, encontramos a tensão após a ponte de diodos de aproximadamente 18.18V e a corrente depois do capacitor de aproximadamente 120mA.

Sabemos que a fonte possui uma corrente alternada de 60Hz, daí obtemos f a partir de 2 * 60 = 120Hz, então basta aplicar a fórmula sobre os valores encontrados.

O resultado desta operação foi de 550uF, porém preferimos comprar um capacitor de 680uF (o segundo valor comercial mais próximo), por segurança.


## Vídeo do projeto
file:///home/gabi/Downloads/WhatsApp%20Video%202024-06-25%20at%2014.51.16.mp4


## Colaboradoes:
Gabriella Almeida - 15528121

Samuel Sandoval Bonachela - 13686282

Joao Victor De Bortoli Prado - 13672071




