# Calcul de la consommation d'un ruban LED en 5V

## 💡 Comment calculer la consommation d'un ruban LED en 5V ?

Nous allons suivre **5 étapes** :
1. **Calcul de la longueur du ruban**
2. **Détermination du nombre total de LED**
3. **Calcul de l'intensité en ampères (A)**
4. **Calcul de la puissance en watts (W)**
5. **Calcul de la consommation annuelle et du coût (€)**

---

## 🔢 1. Longueur du ruban LED

On place les LED **derrière l'écran**, à **2,5 cm du bord**.

**Formule :**
```math
\text{Longueur LED} = 2 \times (\text{Largeur écran} + \text{Hauteur écran}) - 2.5 \times 4
```

---

## 🔢 2. Nombre total de LED

Le ruban a **30 LED/m** ou **60 LED/m**.

**Formule :**
```math
\text{Nombre total de LED} = \text{Longueur LED} \times \text{LED/m}
```

---

## 🔢 3. Intensité totale en ampères (A)

Chaque LED consomme **60 mA = 0.060 A**.

**Formule :**
```math
\text{Intensité} (A) = \text{Nombre total de LED} \times 0.060
```

---

## 🔢 4. Puissance en watts (W)

On utilise la loi de l'électricité :
```math
P = U \times I
```

Avec **U = 5V**, on a :
```math
\text{Puissance} (W) = 5V \times \text{Intensité} (A)
```

---

## 🔢 5. Consommation annuelle et coût (€)

### 🔹 Consommation annuelle (kWh)
```math
\text{Conso annuelle} = \frac{\text{Puissance} (W) \times \text{Heures par jour} \times 365}{1000}
```

### 🔹 Coût annuel (€)
```math
\text{Coût annuel} = \text{Conso annuelle} (kWh) \times \text{Prix du kWh} (€)
```

---

## 📏 Tableau des calculs pour différentes tailles d'écrans

| **Taille écran** | **Largeur (cm)** | **Hauteur (cm)** | **Longueur LED (m)** | **Nombre de LED (30 LED/m)** | **Nombre de LED (60 LED/m)** | **Intensité (A, 30 LED/m)** | **Intensité (A, 60 LED/m)** | **Puissance (W, 30 LED/m)** | **Puissance (W, 60 LED/m)** |
|------------------|-----------------|------------------|-----------------|----------------------|----------------------|----------------------|----------------------|----------------------|----------------------|
| **24 pouces**   | 53.1 cm          | 29.9 cm         | **1.59 m**      | **47 LEDs**          | **95 LEDs**          | **2.86 A**           | **5.74 A**           | **14.3 W**           | **28.7 W**           |
| **27 pouces**   | 59.8 cm          | 33.6 cm         | **1.79 m**      | **54 LEDs**          | **107 LEDs**         | **3.22 A**           | **6.44 A**           | **16.1 W**           | **32.2 W**           |
| **32 pouces**   | 69.8 cm          | 39.3 cm         | **2.09 m**      | **63 LEDs**          | **125 LEDs**         | **3.76 A**           | **7.52 A**           | **18.8 W**           | **37.6 W**           |

*(Basé sur des écrans **16:9** standard.)*

---

## 🔢 Exemple de calcul pour un écran 27 pouces, ruban 60 LED/m, 5h/jour

1. **Longueur du ruban :**
   ```math
   (59.8 + 33.6) \times 2 - (2.5 \times 4) = 1.79 m
   ```

2. **Nombre total de LED :**
   ```math
   1.79 \times 60 = 107 \text{ LED}
   ```

3. **Intensité totale (5V) :**
   ```math
   107 \times 0.060 = 6.44 A
   ```

4. **Puissance totale :**
   ```math
   P = 5V \times 6.44A = 32.2 W
   ```

5. **Consommation annuelle :**
   ```math
   \frac{32.2 \times 5 \times 365}{1000} = 58.8 \text{ kWh}
   ```

6. **Coût annuel (€) :**
   ```math
   58.8 \times 0.20 = 11.85 €
   ```

**💡 Conclusion :** Pour cet écran, un ruban **60 LED/m en 5V** consommera **6.44 A**, et coûtera **11.85 €/an** pour **5h d'utilisation quotidienne**.

---

## 💡 Résumé rapide

1. **Calcul du périmètre – 2,5 cm sur chaque côté.**
2. **Multipliez par 30 LED/m ou 60 LED/m.**
3. **Multipliez par 60 mA pour obtenir l'ampérage.**
4. **Multipliez par 5V pour obtenir la puissance en watts.**
5. **Multipliez par les heures/jour × 365 pour la conso annuelle.**
6. **Multipliez par le prix du kWh pour obtenir le coût annuel.**

---

Si vous voulez un **calcul personnalisé**, utilisez les formules ci-dessus et adaptez à votre besoin !

