Pràctica UD10: Servidor de fitxers amb Samba
Descripció general de la tasca
Aquesta pràctica consisteix en la configuració d'un servidor de fitxers Samba en un entorn de xarxa mixt, on conviuen sistemes Linux (Ubuntu Server i Zorin) i Windows 11. L'objectiu principal és aprendre a compartir recursos (carpetes i fitxers) entre diferents sistemes operatius utilitzant el protocol SMB/CIFS.

Objectius de la pràctica
Instal·lar i configurar un servidor Samba en Ubuntu Server

Crear i gestionar usuaris específics per a Samba

Configurar diferents tipus d'accés a carpetes compartides:

Accés anònim (només lectura)

Accés a carpetes personals dels usuaris

Accés amb permisos diferenciats (lectura/escriptura)

Restringir l'accés a determinats tipus d'arxius (com ara .zip)

Connectar clients Windows i Linux als recursos compartits

Accedir des de Linux a recursos compartits de Windows

Estructura de la pràctica
La pràctica es divideix en 5 exercicis que es desenvolupen de manera progressiva:

Exercici 1: Instal·lació i configuració bàsica
En aquest primer exercici es prepara el servidor. S'instal·la el programari Samba, es creen les carpetes que es compartiran (publica i compartida) amb els permisos adequats, es creen tres usuaris específics (samba1, samba2, samba3) i s'afegeixen a la base de dades de Samba. També es realitza una còpia de seguretat del fitxer de configuració original.

Exercici 2: Carpeta pública en mode anònim
Es configura una primera carpeta compartida (publica) que serà accessible per qualsevol usuari sense necessitat d'autenticació. Aquesta carpeta està configurada només en mode lectura, és a dir, els usuaris podran veure i obrir els fitxers però no modificar-los ni eliminar-los. Es comprova l'accés des de diferents clients.

Exercici 3: Carpetes personals dels usuaris
S'activa la funcionalitat que permet que cada usuari pugui accedir a la seva pròpia carpeta personal del servidor Linux. Aquest accés és amb tots els permisos (lectura i escriptura), de manera que cada usuari pot gestionar lliurement els seus propis fitxers. La carpeta personal de cada usuari només és visible i accessible per al propi usuari.

Exercici 4: Carpeta compartida amb permisos diferenciats
Aquest és l'exercici més complet. Es configura una carpeta (compartida) on s'estableixen diferents nivells d'accés segons l'usuari:

samba1: té permisos de lectura i escriptura

samba2: només pot llegir, no pot modificar res

samba3: no té cap tipus d'accés a aquesta carpeta

A més, s'aplica una restricció addicional: es prohibeix l'accés a arxius amb extensió .zip, de manera que aquests fitxers no es mostren ni es poden accedir des dels clients, tot i que físicament existeixen al servidor.

Exercici 5: Accés de Linux a recursos de Windows
En aquest últim exercici s'inverteixen els papers. Es crea una carpeta compartida a la màquina Windows 11 amb permisos de lectura per a tothom, i des del client Zorin (Linux) s'accedeix a aquest recurs. D'aquesta manera es demostra que la comunicació és bidireccional: tant Windows pot accedir a Linux com Linux pot accedir a Windows.