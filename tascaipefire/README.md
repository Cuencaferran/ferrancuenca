# Tasca IPFire: Configuració de Proxy Web i Filtre de Continguts

## Objectiu
Configurar un servidor IPFire per a actuar com a **proxy web** amb **filtre d’URL**, bloquejant continguts per categories, llistes negres personalitzades i paraules clau, a més d’establir **regles de tallafoc** amb restriccions horàries.

## Materials utilitzats
- IPFire 2.29 (x86_64) amb interfícies **GREEN** (192.168.4.254/24) i **RED** (10.0.2.12/24)
- Client a la xarxa GREEN amb IP 192.168.4.1
- Navegador per accedir al panell de control `https://192.168.4.254:444`
