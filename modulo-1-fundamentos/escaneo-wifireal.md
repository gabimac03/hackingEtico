# Escaneo de red Wi-Fi real (Modo Bridge) - Módulo 1

## 🖥 IP asignada a Kali:

```bash
inet 192.168.100.37/24
```

🌐 Rango escaneado:

nmap -sn 192.168.100.0/24

📋 Dispositivos detectados:

| IP             | Estado | Latencia | MAC Address             | Fabricante          |
| -------------- | ------ | -------- | ----------------------- | ------------------- |
| 192.168.100.1  | Activo | 0.12s    | D8:68:52:6E\:E2:23      | Huawei Technologies |
| 192.168.100.10 | Activo | 0.30s    | 6A:98:36\:B8:88:85      | Unknown             |
| 192.168.100.16 | Activo | 2.4s     | 5A\:E9\:D8:2A\:EF\:AA   | Unknown             |
| 192.168.100.24 | Activo | 0.63s    | 62:5D:0D:2B:12\:D0      | Unknown             |
| 192.168.100.25 | Activo | 0.00049s | 00:45\:E2\:E4:99\:D1    | CyberTAN Technology |
| 192.168.100.34 | Activo | 0.73s    | D2:20:8D:9C:8A:14       | Unknown             |
| 192.168.100.37 | Activo | -        | (Mi máquina Kali Linux) |                     |

## 📝 Notas:
El escaneo se realizó desde una VM Kali Linux en modo "adaptador puente".
Permite identificar dispositivos reales conectados al router Wi-Fi.
Ideal para auditorías internas o pruebas de penetración en redes domésticas.