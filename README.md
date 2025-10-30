Este arquivo manifest.yml contém a configuração para criar um ambiente de laboratório na plataforma Kubernetes hackinsdn. Ele descreve a topologia de rede necessária para simular um cenário de teste de invasão.

A configuração inclui:

Máquina Atacante (kali-attacker): Um contêiner baseado na imagem oficial do Kali Linux (kalilinux/kali-rolling) com o endereço IP 192.168.0.10.

Máquina Alvo (metasploitable-target): Um contêiner vulnerável por design, baseado na imagem tleemcjr/metasploitable2, com o endereço IP 192.168.0.20.

Conectividade: Ambas as máquinas são interligadas em uma rede virtual privada, permitindo a comunicação direta entre elas.

O objetivo é utilizar a máquina Kali para realizar testes de exploração de vulnerabilidades contra a máquina Metasploitable em um ambiente controlado.
