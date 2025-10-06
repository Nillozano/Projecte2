# T03: Seguretat Lògica — Recuperant accés a sistemes

## 🛠️ Descripció del projecte

Després d’una primera feina exitosa, la consultora rep un encàrrec urgent: recuperar l’accés a un portàtil amb **Zorin OS** (una distribució Linux amb entorn gràfic) utilitzat per un directiu que ha oblidat la contrasenya. L’equip conté documentació crítica.

Per evitar riscos, s’ha clonat el disc dur original en un **disc virtual**, i se us demana que treballeu sobre una **màquina virtual**.

## 🎯 Objectius

- Recuperar l’accés al sistema operatiu modificant la contrasenya de l’usuari.
- Investigar i aplicar mesures de **seguretat lògica** per evitar que es pugui repetir aquest procediment en cas de robatori.
- Documentar tot el procés amb imatges i explicacions clares.

## 📋 Tasques a realitzar

### 1. Creació de la màquina virtual

- Crear una màquina virtual amb el disc virtual proporcionat pel client.
- Assegurar que el sistema arrenca correctament.

### 2. Vulneració de l’accés al GRUB

- Accedir al GRUB (el gestor d’arrencada de Linux).
- Modificar els paràmetres d’arrencada per accedir al sistema sense contrasenya.

### 3. Identificació de l’usuari

- Un cop dins del sistema, identificar el nom d’usuari actiu.
- Utilitzar comandes com `ls /home` o `cat /etc/passwd` per localitzar-lo.

### 4. Modificació de la contrasenya

- Assignar una nova contrasenya a l’usuari amb la comanda `passwd nom_usuari`.
- Verificar que l’usuari pot accedir al sistema amb la nova contrasenya.

### 5. Fortificació del GRUB

- Investigar com protegir l’accés al GRUB amb contrasenya.
- Evitar que es pugui modificar la configuració d’arrencada sense autorització.
- Fonts recomanades:
  - [Recuperant Password en Linux](https://waytoit.wordpress.com/2013/06/06/recuperando-password-en-ubuntu/)
  - Apunts **RA1AA4 Seguretat Lògica**

### 6. Configuració de seguretat

- Aplicar la protecció al GRUB a la màquina virtual.
- Verificar que el sistema no permet accedir ni modificar el GRUB sense credencials.

### 7. Documentació del procediment

- Crear un document amb:
  - Captures de pantalla de cada pas
  - Explicacions detallades
  - Fonts consultades
- Pujar el document al repositori personal.

## 📚 Material de suport

- Disc virtual del client
- Apunts RA1AA4 Seguretat Lògica
- Guia online: [Recuperant Password en Linux](https://waytoit.wordpress.com/2013/06/06/recuperando-password-en-ubuntu/)

---
