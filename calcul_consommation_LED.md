# Calcul de la consommation d'un ruban LED en 5V

## 💡 Comment calculer la consommation du ruban LED en 5V ?

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
   58.8 \times 0.2016 = 11.85 €
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

---
# 🔌 Calculateur automatique de consommation des LED 💡

Simplifiez-vous la vie avec ce code HTML + JavaScript ! Il vous permet de calculer automatiquement plusieurs paramètres liés à l’utilisation des rubans LED. Il suffit de le copier-coller dans un éditeur HTML en ligne ou sur votre propre site pour effectuer les calculs en quelques secondes.

## 📊 Ce que ce calculateur permet d’évaluer :

✅ Longueur du ruban LED requise (en mètres) en fonction des dimensions réelles de l’écran.  
✅ Nombre total de LED en fonction du type de ruban choisi (30 ou 60 LED/m).  
✅ Intensité électrique totale consommée (en ampères).  
✅ Puissance totale utilisée par le ruban (en watts).  
✅ Consommation énergétique quotidienne (en kWh).  
✅ Coût annuel d’utilisation basé sur le prix du kWh renseigné.  

---

## 📌 Mode d’emploi :
1️⃣ Entrez la largeur et la hauteur **réelles** de l’écran en centimètres.  
2️⃣ Sélectionnez le type de LED (30 ou 60 LED/m).  
3️⃣ Indiquez le nombre d’heures d’utilisation par jour.  

---

## 🖥️ Code HTML + JavaScript :

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calcul de Consommation LED</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            padding: 20px;
            max-width: 500px;
            margin: auto;
        }
        input, select, button {
            display: block;
            width: 100%;
            margin-bottom: 10px;
            padding: 8px;
            font-size: 16px;
        }
        .result {
            font-size: 18px;
            margin-top: 20px;
            padding: 10px;
            background: #f4f4f4;
            border-left: 5px solid #007BFF;
        }
    </style>
</head>
<body>
    <h1>Calcul de Consommation des LED</h1>
    
    <label for="largeur">Largeur de l'écran (cm) :</label>
    <input type="number" id="largeur" placeholder="Entrez la largeur" required>

    <label for="hauteur">Hauteur de l'écran (cm) :</label>
    <input type="number" id="hauteur" placeholder="Entrez la hauteur" required>

    <label for="typeLED">Type de LED (30 ou 60 LEDs/m) :</label>
    <select id="typeLED">
        <option value="30">30 LEDs/m</option>
        <option value="60">60 LEDs/m</option>
    </select>

    <label for="temps">Temps d'utilisation par jour (heures) :</label>
    <input type="number" id="temps" placeholder="Entrez le temps d'utilisation" required>

    <label for="prix">Prix du kWh (€) :</label>
    <input type="number" id="prix" placeholder="Entrez le prix du kWh" required>

    <button onclick="calculer()">Calculer</button>

    <div class="result" id="result"></div>

    <script>
        function calculer() {
            var largeur = parseFloat(document.getElementById("largeur").value);
            var hauteur = parseFloat(document.getElementById("hauteur").value);
            var typeLED = parseInt(document.getElementById("typeLED").value);
            var temps = parseFloat(document.getElementById("temps").value);
            var prix = parseFloat(document.getElementById("prix").value);

            if (isNaN(largeur) || isNaN(hauteur) || isNaN(temps) || isNaN(prix)) {
                alert("Veuillez remplir tous les champs avec des valeurs valides.");
                return;
            }

            var longueurLED = 2 * (largeur + hauteur) / 100 - 2.5 * 4 / 100;
            var nombreLEDs = longueurLED * typeLED;
            var ampereTotal = nombreLEDs * 0.060;
            var puissanceTotaleW = ampereTotal * 5;
            var consommationKWhJour = puissanceTotaleW * temps / 1000;
            var coutAnnuel = consommationKWhJour * 365 * prix;

            document.getElementById("result").innerHTML = `
                <p><strong>Longueur du ruban LED :</strong> ${longueurLED.toFixed(2)} m</p>
                <p><strong>Nombre total de LED :</strong> ${nombreLEDs}</p>
                <p><strong>Intensité totale :</strong> ${ampereTotal.toFixed(2)} A</p>
                <p><strong>Puissance totale :</strong> ${puissanceTotaleW.toFixed(2)} W</p>
                <p><strong>Consommation journalière :</strong> ${consommationKWhJour.toFixed(3)} kWh</p>
                <p><strong>Coût annuel :</strong> ${coutAnnuel.toFixed(2)} €</p>
            `;
        }
    </script>
</body>
</html>
```
---
Voici, par exemple, un site pour tester le code : [OneCompiler](https://onecompiler.com/html/3y5x8jr6s).


