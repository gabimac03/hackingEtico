# OSINT sobre subdominio de Tienda Nube: entremontanas.mitiendanube.com

## Dominio raíz: mitiendanube.com

- Registrador: Marcaria International LLC
- Creación: 2015-07-21
- Expira: 2026-07-21
- DNS: AWS (Amazon Web Services)
- DNSSEC: No firmado

---

## Subdominio: entremontanas.mitiendanube.com

### NSLOOKUP

```bash
nslookup entremontanas.mitiendanube.com
```
- CNAME → nlb-fallback.mitiendanube.com.cdn.cloudflare.net
- IPs resultantes: 185.133.35.13, 185.133.35.14

### DIG

dig entremontanas.mitiendanube.com
Confirma el alias CNAME

IPs apuntan a Cloudflare

TTL corto (respuesta de 51 a 108 segundos)

### WhatWeb

whatweb entremontanas.mitiendanube.com
Web Server: Cloudflare

HTTPS: Forzado (redirección 301)

Headers de seguridad: CSP, STS, X-XSS, etc.

Recursos detectables: íconos de medios de pago, imágenes de tienda

Plataforma detectada: HTML5 + scripts de JSON y OG

Título de página: "Tienda Online de Entre Montañas"

## Conclusión

El dominio y subdominio están protegidos mediante Cloudflare y AWS.
No se detectan tecnologías vulnerables ni configuraciones incorrectas.
La tienda se beneficia del aislamiento de Tienda Nube, pero su visibilidad técnica es limitada.