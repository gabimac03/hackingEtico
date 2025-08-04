# Informe OSINT Pasivo - <dominio objetivo>

## 🧾 1. Información general

- **Dominio analizado**: <dominio>
- **Fecha del análisis**: <fecha>
- **Tipo de objetivo**: (Empresa / Tienda / Gobierno / Otro)
- **Subdominios de interés**: 
  - <sub1.dominio>
  - <sub2.dominio>
- **Observaciones iniciales**: 
  - (Ej: Se trata de una tienda sobre Tienda Nube con redirección a HTTPS y protección de Cloudflare)

---

## 🔍 2. WHOIS

```bash
whois <dominio>
```

- Registrador: <Marcaria / Cloudflare / GoDaddy / etc.>
- Fecha de creación: <yyyy-mm-dd>
- Fecha de vencimiento: <yyyy-mm-dd>
- DNSSEC: (Sí / No)
- Servidores NS:
ns1...
ns2...
- Privacidad WHOIS: (Sí / No)
- Estado del dominio: (clientTransferProhibited, etc.)

## 🌐 3. DNS y resolución - NSLOOKUP
```bash
nslookup <dominio o subdominio>
```
- IPs detectadas:

IPv4: <ip>
IPv6: <ip>

- Alias (CNAME): <si aplica>

## DIG 
``` bash
dig <dominio> any
Registros encontrados:
```

- A: <ip>
- MX: <registro si aplica>
- CNAME: <alias si aplica>
- TXT/SPF: <datos si los hay>

## 🧠 4. Análisis de tecnologías (WhatWeb)
```bash
whatweb <dominio>
```

- Servidor web: <Apache / Nginx / Cloudflare>
- CMS / Plataforma: <WordPress / Drupal / HTML5 puro / No detectado>
- HTTPS / Redirecciones: (Sí / No, tipo de redirección)
- Headers de seguridad:

X-Frame-Options: ...

Strict-Transport-Security: ...

Content-Security-Policy: ...

Otros encabezados detectados:

## 🧭 5. theHarvester (si se usó)

```bash
theHarvester -d <dominio> -b <bing/linkedin/yahoo/crtsh>
```

- Emails detectados:

(Si hay, listarlos)

- Hosts detectados:

(Si hay, listarlos)

- Subdominios / IPs:

## 🔎 6. Google Dorks (manual)

site:<dominio> filetype:pdf

inurl:admin site:<dominio>

intitle:"index of" site:<dominio>


## 🔐 7. Certificados SSL (crt.sh)
Buscado en: https://crt.sh

Subdominios expuestos por certificados públicos:
...

Observaciones:
...