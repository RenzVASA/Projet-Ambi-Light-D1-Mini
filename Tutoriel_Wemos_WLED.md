# 🚀 Tutoriel : Installer et Flasher WLED sur un Wemos D1 Mini

## 📌 1. Installation de l’IDE Arduino

### 📥 Télécharger l'IDE Arduino
- Rendez-vous sur le site officiel : [Télécharger Arduino IDE](https://www.arduino.cc/en/software)
- Installez la version correspondant à votre système (Windows, macOS, Linux).

### 🔧 Ajouter le support ESP8266
1. **Ouvrez Arduino IDE** et allez dans **Fichier > Préférences**.
2. Dans "URL de gestionnaire de cartes supplémentaires", ajoutez cette URL :
   ```
   http://arduino.esp8266.com/stable/package_esp8266com_index.json
   ```
3. Cliquez sur **OK**.
4. Allez dans **Outils > Type de carte > Gestionnaire de cartes**.
5. Recherchez **esp8266**, installez **"esp8266 by ESP8266 Community"**.

---

## 🔌 2. Connecter et Configurer le Wemos D1 Mini

### 📡 Sélectionner la carte et le port
1. Branchez votre **Wemos D1 Mini** en USB à votre PC.
2. Dans **Outils > Type de carte**, sélectionnez **LOLIN(WEMOS) D1 R2 & mini**.
3. Dans **Outils > Port**, sélectionnez le port COM correspondant à votre Wemos.

---

## 🔍 3. Récupérer l’Adresse MAC du Wemos

1. **Créez un nouveau sketch** dans l’IDE Arduino.
2. **Copiez-collez ce code** dans l'éditeur :

   ```cpp
   #include <ESP8266WiFi.h>

   void setup() {
       Serial.begin(115200);
       delay(1000);
       Serial.println();
       Serial.print("Adresse MAC : ");
       Serial.println(WiFi.macAddress());
   }

   void loop() {
   }
   ```

3. **Téléversez** le code sur la carte en cliquant sur 🔼 (flèche vers la droite).
4. **Ouvrez le Moniteur Série** via **Outils > Moniteur Série** (vitesse : **115200 bauds**).
5. **L’adresse MAC s'affichera**, exemple :
   ```
   Adresse MAC : XX:XX:XX:XX:XX:XX
   ```

---

## 🔥 4. Flasher WLED sur le Wemos

### 🌍 Accéder au site de flashage
- Ouvrez **Google Chrome** ou **Edge**.
- Rendez-vous sur : [https://install.wled.me](https://install.wled.me)

### 🚀 Flashage du Wemos
1. Cliquez sur **Install WLED**.
2. Sélectionnez le **Wemos D1 Mini** dans la liste des ports USB.
3. Suivez les instructions pour **installer le firmware WLED**.

---

## ✅ 5. Finalisation
- Une fois installé, votre Wemos créera un réseau **WLED-AP**.
- Connectez-vous avec votre téléphone/PC et configurez-le ! 🎨✨

## 🔥 6. Flasher WLED avec la bonne version

### 📌 a. Sélectionner la version de WLED
- Sur la page [install.wled.me](https://install.wled.me), clique sur **Install WLED**.
- Il te propose plusieurs versions :
  - **Prends la dernière version stable** (évite les versions bêta pour plus de stabilité).
  - Exemple : **WLED 0.xx.xx Release**.

### 📌 b. Choisir le bon firmware
- Sélectionne **Plain (Generic ESP8266)**.
- C’est l’option classique qui fonctionne pour le **Wemos D1 Mini**.

### 📌 c. Sélectionner le port série
- **Branche ton Wemos D1 Mini** à ton PC avec un bon câble USB (**data**, pas juste charge).
- Dans la liste des **Serial Ports**, choisis celui qui ressemble à :
  - **"COMX"** (Windows) où **X** est un chiffre.
  - **"/dev/ttyUSBX"** (Linux/Mac).

- **Si aucun port ne s’affiche** :
  - Vérifie que ton **câble permet bien le transfert de données**.
  - Essaie un **autre port USB** ou un **autre câble**.
  - Installe le **driver CH340** si nécessaire (le Wemos D1 Mini utilise souvent ce chipset) :
    - [Driver CH340 pour Windows/Mac/Linux](https://www.wch.cn/downloads/CH341SER_EXE.html)
   
      
## ⚡ 7. Lancer l’installation de WLED
- **Clique sur Install** et laisse le processus se terminer (**environ 1 à 2 minutes**).
- Une fois terminé, ton **Wemos va redémarrer** et créer un réseau Wi-Fi **"WLED-AP"**.


📌 **Besoin d'aide ?** Posez-moi tes questions ! 🚀😃


