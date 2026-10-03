# Ambi-Light D1 Mini

Un éclairage d'ambiance piloté en Wi-Fi, avec un microcontrôleur Wemos D1 Mini (ESP8266), le firmware WLED et une bande LED WS2812B.

<img src="Images/Sche%CC%81ma-D1.jpg" alt="Schéma de câblage : alimentation USB 5 V, Wemos D1 Mini et bande LED WS2812B" width="100%">

## La documentation

1. **[Flasher WLED sur le D1 Mini](installation_WLED-D1.md)** : installer le firmware depuis le navigateur.
2. **[Trouver l'adresse MAC du Wemos](GET_MAC_WEMOS.md)** : pour le réserver sur le réseau.
3. **[Le schéma de câblage](Wemos_LED_Schema.md)** : alimentation 5 V, masse commune, ligne de données.
4. **[Calculer la consommation](calcul_consommation_LED.md)** : choisir la bonne alimentation selon le nombre de LED.

## Matériel

- Wemos D1 Mini (ESP8266)
- Bande LED adressable WS2812B
- Alimentation 5 V adaptée au nombre de LED
- Câble USB **data** (pas seulement charge) pour le flashage

## Ce que j'ai fait

Choix des composants, schéma sous Proteus 8, soudure, calcul de consommation et configuration de WLED.

---

Fait par [RenzVASA](https://renzvasa.github.io).
