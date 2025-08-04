# Módulo 1 - Comandos Básicos en Kali Linux

## Información del sistema

```bash
whoami
# adminn

hostname
# vbox

Red

ip a
# Dirección IP local: 10.0.2.15 (adaptador eth0)
ping 8.8.8.8
# 31 paquetes transmitidos, 31 recibidos, 0% pérdida
# Promedio de latencia: ~67 ms

Puertos abiertos

netstat -tuln
# Muestra servicios activos en escucha en diferentes puertos

```

## Notas 
- El adaptador eth0 es el principal para conexión a Internet en VirtualBox.
- La IP 10.0.2.15 indica que estás usando NAT (Network Address Translation) como modo de red.
- netstat requiere net-tools; si no estuviera instalado, usar:
sudo apt update
sudo apt install net-tools


