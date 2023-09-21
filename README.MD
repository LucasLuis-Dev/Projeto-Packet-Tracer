<img src="https://cdn.discordapp.com/attachments/965066624556232737/1115030737805136043/Design_sem_nome.png">

# Projeto Packet Tracer | Redes de Computadores - IF975

Este projeto foi desenvolvido como parte da disciplina de Redes de Computadores ministrada pelo professor Dr. Kelvin Lopes no Centro de Informática da UFPE. 

Nele, criei um sistema para uma rede empresarial utilizando a plataforma Cisco Packet Tracer. O objetivo principal era criar três redes distintas, cada uma representando um departamento diferente da empresa. Cada departamento foi equipado com seu próprio roteador e utilizou o protocolo OSPF para facilitar a comunicação entre eles. Além disso, foram implementados servidores DHCP em cada sub-rede para atribuição automática de endereços IP aos dispositivos.


## Imagens das Rotas nos Roteadores

ALOCAÇÕES DE IPs REALIZADAS NO PROJETO

## Alocações de IPs Realizadas no Projeto

IPs Alocados para a Rede do Departamento 1:
- Rede do Departamento 1: 192.168.0.0/24
- IP do Roteador na Rede do Departamento: 192.168.0.1
- IP do Roteador do Departamento para o roteamento: 10.0.0.1
- IP do DHCP: 192.168.0.2

IPs Alocados para a Rede do Departamento 2:
- Rede do Departamento 2: 192.168.1.0/24
- IP do Roteador na Rede do Departamento: 192.168.1.1
- IP do Roteador  para o roteamento entre o departamento 1 e 2 : 10.0.0.2
- IP do Roteador para o roteamento entre os departamentos 2 e 3: 10.0.1.1
- IP do DHCP: 192.168.1.2

IPs Alocados para a Rede do Departamento 3:
- Rede do Departamento 3: 192.168.2.0/24
- IP do Roteador na Rede do Departamento: 192.168.2.1
- IP do Roteador para o Roteamento entre os Departamentos 3 e 2: 10.0.1.2
- IP do DHCP: 192.168.2.2

Rede dos Roteadores dos Departamentos 1 e 2: 10.0.0.0/24
Rede dos Roteadores dos Departamentos 2 e 3: 10.0.1.0/24



## Comandos Usados no Projeto

Comandos usados para a configuração do roteamento usando OSPF

1. enable
2. configure terminal
3. router ospf [Número do Processo OSPF]
4. network [Endereço de Rede] [Wildcard] area [Número da Área OSPF]
5. end
6. write memory
7. show ip ospf neighbor


As demais configurações como o DHCP, Endereços IPs, VLANs foram feitas através da própria interface gráfica do Packet Tracer, por isso não houve a utilização de mais comandos no projeto


## Vídeo Demonstrativo do Funcionamento do Projeto


Neste vídeo eu busco mostrar o funcionamento do projeto de forma mais clara mostrando desde o roteamento até o funcionamento das VLANs que pode ser reparado no vídeo que o único pacote que deu “Failed” foi justamente um pacote de uma máquina que tentou ser enviado para outra máquina em uma VLAN diferente .

<a href="google.com">
    <img src="https://cdn.discordapp.com/attachments/965066624556232737/1154234922568003624/Captura_de_tela_2023-09-20_225659.png">
<a/>