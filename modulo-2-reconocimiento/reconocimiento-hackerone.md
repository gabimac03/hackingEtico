# OSINT sobre dominio real: hackerone.com

## WHOIS

- Registrador: Cloudflare, Inc.
- Creado: 2007-11-26
- Expira: 2025-11-26
- DNSSEC: Activado
- Estado del dominio: Protegido contra edición y transferencia
- Servidores DNS: a.ns.hackerone.com, b.ns.hackerone.com

## DNS Lookup (nslookup & dig)

- IPv4: 104.18.36.214, 172.64.151.42
- IPv6: 2606:4700:4400::ac40:972a, 2606:4700:4400::6812:24d6
- Balanceo de carga y protección por Cloudflare

## TheHarvester

- Herramienta: `theHarvester -d hackerone.com -b bing`
- Resultado: sin datos públicos detectables desde Bing
- Posible explicación: uso de protección de correos y subdominios

## WhatWeb

- Tecnologías detectadas:
  - CMS: Drupal
  - Webserver: Cloudflare
  - Headers de seguridad: CSP, X-Frame-Options, STS, etc.
  - Redirecciones correctas: http → https → www

## Conclusión

- HackerOne es un ejemplo de buena configuración de seguridad pasiva.
- No se detectaron correos o subdominios por fuentes públicas.
- Protecciones como Cloudflare, DNSSEC, y encabezados de seguridad están activas.