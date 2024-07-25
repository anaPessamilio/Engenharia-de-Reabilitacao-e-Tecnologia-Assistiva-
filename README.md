# Projeto de Controle de Cadeira de Rodas via Aplicativo

## Introdução

Durante a disciplina, o grupo identificou as dificuldades enfrentadas por pessoas usuárias de cadeiras de rodas, especialmente em situações em que a cadeira não está facilmente acessível. Pensando na independência e inclusão, o projeto final desenvolvido consiste em um sistema que permite controlar uma cadeira de rodas por meio de um aplicativo no celular, trazendo a cadeira até o usuário.

## O Projeto

O protótipo desenvolvido é um carrinho controlado via aplicativo celular, equipado com dois motores e um sensor ultrassônico para evitar colisões. O aplicativo possui uma interface simples com 5 botões para controlar o movimento da cadeira: Frente, Trás, Direita, Esquerda e Frear.

### Materiais

- Kit chassi para robô de duas rodas
- Driver motor ponte H - L298N
- Módulo NodeMCU ESP-12E com WiFi V3
- Sensor ultrassônico
- 8 pilhas AA para alimentação do ponte H
- 1 pilha de 3V para alimentação do ESP32
- Protoboard, cabos e jumpers para montagem do circuito

## Desenvolvimento

### Aplicativo

O aplicativo foi desenvolvido usando as seguintes ferramentas:

- **Visual Studio Code**: Editor de código-fonte com suporte para depuração e controle de versionamento Git.
- **Expo-Client**: Ferramenta para criação de apps universais em React Native e execução em dispositivos físicos.
- **React Native**: Framework para transformação de código JavaScript e TypeScript em código nativo para Android e iOS.

**Interface:** Composta por 5 botões para controlar o movimento da cadeira, dispostos de forma intuitiva.

**Scripts:** O aplicativo envia requisições HTTP para o servidor ESP, que aciona os motores de acordo com o comando recebido.

**Controle do Carrinho:** O carrinho utiliza um sensor ultrassônico para detectar obstáculos. Se um obstáculo for detectado a uma distância menor que um valor pré-determinado, o carrinho freia.

**Montagem do Circuito:** O circuito foi montado em cima do chassi do carrinho, com componentes organizados e fixados adequadamente.

**Resultados:** O tempo de resposta do carrinho após um comando é geralmente inferior a 0.5 segundos. A resposta a obstáculos é inferior a 0.2 segundos. No entanto, o carrinho apresenta pequenas folgas e desalinhamentos que afetam o movimento.

### Conclusão

O protótipo desenvolvido conseguiu atender ao objetivo de criar um sistema de adaptação para cadeiras de rodas, possibilitando a solução da problemática apresentada. O grupo está satisfeito com o resultado e acredita que o projeto está bem alinhado com os conceitos aprendidos na disciplina.
