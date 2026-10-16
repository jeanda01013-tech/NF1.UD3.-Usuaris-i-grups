# NF1.UD3.-Usuaris-i-grups

![foto1](/capturas_extraidas/capturas_extraidas/captura_01.png)

- En aquesta captura es comprova que els tres grups han estat creats correctament. També podeu identificar els vostres respectius GID al fitxer /etc/group.


![foto1](/capturas_extraidas/capturas_extraidas/captura_02.png)

- S'ha modificat el .bashrc de /etc/skel perquè els usuaris nous disposin automàticament de l'àlies ll.

![foto1](/capturas_extraidas/capturas_extraidas/captura_03.png)

- La configuració DSHELL=/bin/bash estableix Bash com a shell predeterminat per als usuaris creats mitjançant adduser.

![foto1](/capturas_extraidas/capturas_extraidas/captura_04.png)

- L'usuari de prova ha heretat correctament els fitxers i directoris configurats prèviament a /etc/skel.

![foto1](/capturas_extraidas/capturas_extraidas/captura_05.png)

- En aquesta captura es comprova la creació dels quatre usuaris i els grups a què pertany cadascun. Marc també pertany al grup secundari devs. 

![foto1](/capturas_extraidas/capturas_extraidas/captura_06.png)

- S'ha configurat el compte de pau_dev perquè la contrasenya s'hagi de canviar obligatòriament a l'inici de sessió següent.

![foto1](/capturas_extraidas/capturas_extraidas/captura_07.png)

- En iniciar sessió com a pau_dev, el sistema obliga a l'usuari a establir una nova contrasenya a causa de la configuració realitzada amb chage.

![foto1](/capturas_extraidas/capturas_extraidas/captura_08.png)

- L'usuari marc_sys té com a grup principal sysadmin i com a grup secundari devs, tal com estableix l'enunciat.

![foto1](/capturas_extraidas/capturas_extraidas/captura_09.png)

- El fitxer /etc/passwd conté informació general dels comptes, com ara el nom d'usuari, UID, GID, nom complet, directori personal i intèrpret d'ordres. La contrasenya no s'emmagatzema directament aquí.

![foto1](/capturas_extraidas/capturas_extraidas/captura_10.png)

- El fitxer /etc/shadow conté informació sensible d'autenticació, com ara el hash de la contrasenya i dades relacionades amb la seva caducitat.

![foto1](/capturas_extraidas/capturas_extraidas/captura_11.png)

- /etc/shadow té permisos restringits perquè conté informació sensible relacionada amb les contrasenyes. Només root i els usuaris autoritzats del grup corresponent han de poder accedir-hi.

![foto1](/capturas_extraidas/capturas_extraidas/captura_12.png)

- /etc/skel és el directori plantilla utilitzat per proporcionar fitxers i configuracions inicials als nous usuaris.

![foto1](/capturas_extraidas/capturas_extraidas/captura_13.png)

- La configuració d'adduser.conf defineix valors predeterminats utilitzats durant la creació de comptes nous, mentre que /etc/skel proporciona els fitxers inicials de l'usuari.

![foto1](/capturas_extraidas/capturas_extraidas/captura_14.png)

- el signe ! afegit davant la informació d'autenticació indica que el compte de pau_dev està bloquejat i no es pot autenticar mitjançant contrasenya.

![foto1](/capturas_extraidas/capturas_extraidas/captura_15.png)

- S'ha desbloquejat novament el compte de pau_dev, permetent que l'usuari pugui iniciar sessió.

![foto1](/capturas_extraidas/capturas_extraidas/captura_16.png)

- L'usuari auditor ha estat eliminat juntament amb el directori personal. D'aquesta manera també s'eliminen els fitxers personals associats al directori /home/auditor.

![foto1](/capturas_extraidas/capturas_extraidas/captura_17.png)

- He instal·lat el fish 

![foto1](/capturas_extraidas/capturas_extraidas/captura_18.png)

- Aquesta és la versió i ho he comprovat 

![foto1](/capturas_extraidas/capturas_extraidas/captura_19.png)

- La comanda which fish mostra que l'intèrpret d'ordres Fish està instal·lat a la ruta /usr/bin/fish.

![foto1](/capturas_extraidas/capturas_extraidas/captura_20.png)

- La comanda echo $SHELL mostra que el shell de l'usuari laura_dev és /bin/bash. Per tant, cal revisar la configuració i tornar a iniciar sessió per comprovar que Fish s'utilitza correctament.