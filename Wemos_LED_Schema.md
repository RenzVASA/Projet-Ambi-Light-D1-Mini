# 🔌 Schéma de connexion Wemos D1 Mini & LED WS2812B  

Ce document présente le schéma de connexion entre un **Wemos D1 Mini**, une **bande LED WS2812B**, et une **alimentation 5V**.  

Les LED WS2812B sont des LED adressables individuellement qui nécessitent une alimentation stable et un signal de commande provenant d'un microcontrôleur comme le Wemos D1 Mini (ESP8266).  

---

## 📜 Matériel requis  
🔹 **Wemos D1 Mini** (ESP8266)  
🔹 **Ruban LED WS2812B** (ex: 30, 60, ou 144 LED/m)  
🔹 **Alimentation 5V** (adaptée à la consommation des LED)    
🔹 **Fils de connexion**  

---

## ⚡ Schéma de connexion  

Le schéma suivant montre comment relier chaque composant :  

![Schéma de connexion](https://github.com/RenzVASA/Projet-Ambi-Light-D1-Mini/blob/main/Images/Sche%CC%81ma-D1.jpg?raw=true)

---

## 🛠️ Instructions de câblage  

1️⃣ **Alimentation**  
   - Connecter le **5V** de l’alimentation au **5V** du ruban LED et au **5V** du Wemos D1 Mini.  
   - Connecter la **masse (GND)** de l’alimentation à la **masse du ruban LED** et au **GND du Wemos**.  

2️⃣ **Signal de contrôle**  
   - Connecter la broche **D4 (GPIO2)** du Wemos à l’entrée **DATA IN** du ruban LED.  

---

## ⚠️ Remarques importantes  

✅ **Utiliser une alimentation adaptée**  
   - Chaque LED WS2812B consomme environ **60mA à pleine luminosité (blanc 100%)**, mais cela varie en fonction de l’intensité et des couleurs utilisées.  
   - Pour calculer précisément l’alimentation nécessaire en fonction de votre installation, consultez [ce fichier de calcul](https://github.com/RenzVASA/Projet-Ambi-Light-D1-Mini/blob/main/calcul_consommation_LED.md).  

✅ **Éviter les longs câbles pour le signal DATA**  
   - Au-delà de **50 cm**, utiliser un fil blindé ou un amplificateur de signal.  
