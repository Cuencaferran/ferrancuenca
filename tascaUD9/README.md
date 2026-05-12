# Tasca: Integració d’un client Linux a un domini Active Directory

## Objectiu

Aprendre a integrar un equip amb sistema operatiu Linux (Zorin OS) dins d’un domini Active Directory, configurant l’autenticació centralitzada mitjançant SSSD i permetent l’accés d’usuaris i grups del domini.

## Requisits previs

- Un servidor Windows Server amb Active Directory configurat i el domini `FOODLOGISTIC.TEST`.
- Un client amb Zorin OS (o qualsevol distribució basada en Ubuntu) connectat a la mateixa xarxa que el servidor AD.
- Credencials d’administrador del domini.
- Accés `sudo` a la màquina Linux.

## Escenari

El departament de logística vol integrar els seus equips Linux a l’entorn Active Directory per centralitzar usuaris, permisos i recursos compartits. En aquesta pràctica s’unirà un equip Zorin al domini `FOODLOGISTIC.TEST` i es configurarà l’accés per a un grup específic d’administradors Linux.
