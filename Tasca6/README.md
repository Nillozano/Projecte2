Ara que ja heu realitzat la formació teòrica, el vostre tutor, t’ha assignat una tasca crucial per a un nou projecte amb un client que necessita modernitzar la seva infraestructura de xarxa.

El client té una xarxa interna que actualment assigna les adreces IP de manera manual, cosa que provoca conflictes d'adreces i una gestió ineficient. L'encàrrec és dissenyar i implementar un servidor DHCP per automatitzar aquest procés, millorant la fiabilitat i reduint la càrrega de treball per als administradors de xarxa. El client ha optat per utilitzar un sistema operatiu Ubuntu Server per a la tasca.

La te missió és la següent:

**Tasques a Realitzar**
**1. Configuració del Servidor:**
- Instal·la el paquet necessari per al servidor DHCP en un servidor Ubuntu.
- Configura el fitxer principal del servei segons el següent pla de disseny:
    - Subxarxa: 192.169.x.0/24 (x teu nº de llista).
    - Rang 192.169.x.100 a 192.169.x.200
    - Porta enllaç 192.169.x.254 i DNS 8.8.8.8
- Configura el servidor per assignar la porta d'enllaç (gateway) i un servidor DNS als clients.
- Reinicia el servei i verifica que s'ha iniciat correctament i sense errors.

**2. Verificació i Proves:**
- Utilitza una màquina client (un Zorin) per connectar-te a la xarxa.
- Captura amb el WireShark els paquets de la negociació entre client i servidor.
- Verifica que el client ha obtingut una adreça IP del servidor DHCP. Comprova que l'adreça IP assignada està dins del rang definit.
- En el client, verifica que la porta d'enllaç i l'adreça del servidor DNS també s'han assignat correctament.
- Per verificar el funcionament de la reserva, incloure la reserva a la configuració del servidor amb l’adreça MAC del client de prova i una IP fora del rang definit, per exemple, 192.169.x.80. Reinicia el servei de xarxa al client i comprova com ha canviat l’adreça a la reserva.

Has de documentar tot el procés en un informe detallat que inclogui:
- Els passos seguits per a la instal·lació i la configuració del servidor.
- Les ordres utilitzades per verificar el correcte funcionament del servei.
- Captures de pantalla del servidor i del client que mostrin la configuració i els resultats de les proves així com dels paquets de la negociació.

**Material de suport**
- Apunts UD2 Configuració servidor DHCP 0227 Serveis de Xarxa (Moodle)
