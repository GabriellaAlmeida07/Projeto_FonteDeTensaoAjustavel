# Projeto_FonteDeTensaoAjustável
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


## Fotos do circuito na protoboard
![2db8313d-9aef-4dc3-9cda-20fbeb00f63c](https://github.com/GabriellaAlmeida07/Projeto_FonteDeTensaoAjustavel/assets/135055000/dde24c35-ba9f-4913-b386-a82c9700a2bf)

![5edc806d-a50e-4728-a3e1-ea7236ce99d1](https://github.com/GabriellaAlmeida07/Projeto_FonteDeTensaoAjustavel/assets/135055000/5375cc83-dd17-4652-a18e-ce20cc00d32c)


## Circuito Falstad
[Circuito Falstad](https://tinyurl.com/2gfmwb9f)

![Captura de tela de 2024-06-26 18-35-03](https://github.com/GabriellaAlmeida07/Projeto_FonteDeTensaoAjustavel/assets/135055000/f7a6e8ca-1972-4801-b328-6e293aa46f53)


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

[![Captura de tela de 2024-06-26 18-40-31](https://github.com/GabriellaAlmeida07/Projeto_FonteDeTensaoAjustavel/assets/135055000/6a0d93af-3fb1-45c2-8d67-d8f7d5a2bb25)](https://youtube.com/shorts/gmYSijptPVI?feature=share)


## Colaboradoes:
Gabriella Almeida - 15528121

Samuel Sandoval Bonachela - 13686282

Joao Victor De Bortoli Prado - 13672071




