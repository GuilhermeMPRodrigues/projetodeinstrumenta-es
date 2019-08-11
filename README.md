Normalmente, vemos drones controlados usando um controle remoto de RF ou, para o piloto automático, usando um módulo de GPS para controlá-lo automaticamente, dando a direção correta por ele.

Como seu nome sugere, o piloto automático significa que o drone será controlado por ele mesmo, enquanto a ação de controle do drone será controlada por um controlador de vôo que tenha sensores embutidos para equilibrar o drone. Um Arduino Uno é o cérebro do sistema, que dá o sinal adequado ao controlador de vôo. Para manter a estabilidade e a operação sustentada, usei um microcontrolador OpenPilot CC3D (ou qualquer controlador de vôo), juntamente com uma câmera para capturar dados ao vivo com sensores de monitoramento meteorológico. Finalmente, o sistema inclui um módulo Bluetooth para ativar / desativar o dronon e exibir os dados ao vivo usando um dispositivo móvel Android.

Arduino Uno:
como sabemos, o arduino Uno é um controlador Atmega Micro. aqui eu gerava sinais PWM para controlar o Drone.

Controlador de vôo CC3D:

O controlador de vôo que possui recursos de giroscópio e controlador de acelerador e nivelamento automático.

Aplicativo móvel:

O aplicativo android que é construído usando um site de código aberto. Usando este aplicativo, podemos ligar e desligar o drone. e ter outro recurso que faz com que possamos obter os dados do sensor na janela serial, ou seja, um telefone celular.

Botões:

start: este botão inicializa o micro controlador

mov: isso faz o drone voar e faz sua operação que é programada dentro do arduino Uno

parar: é um botão de parada de emergência para desligar o drone (devido ao piloto automático drone nenhum controlador remoto está presente assim que fornecido botão extra)

start sensor: quando pressionado, exibe os dados dos sensores em uma tela branca

A temperatura e a umidade dos valores serão exibidas quando o botão do sensor de partida for pressionado.
