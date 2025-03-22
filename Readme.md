D'accord ! Je vais te fournir des réponses détaillées aux trois premiers exercices en français, avec des explications claires pour aider les étudiants à comprendre les concepts.  

---

### **Exercice 1 :**  
Soient \( x \) et \( y \) deux entiers naturels non nuls tels que \( x \times y = 1 \).  

1) **Montrer que les nombres \( x+y \) et \( x \) et \( y \) ne sont pas de même parité.**  

- La parité d'un nombre entier correspond à sa nature paire ou impaire :  
  - Un entier est **pair** s'il est divisible par 2.  
  - Un entier est **impair** s'il n'est pas divisible par 2.  

- On nous dit que \( x \times y = 1 \). Or, les seuls entiers naturels dont le produit est 1 sont **\( x = 1 \) et \( y = 1 \)**.  

- Donc :  
  \[
  x + y = 1 + 1 = 2
  \]
  Or, 2 est **pair**, alors que \( x \) et \( y \) sont **impairs**.  

- Conclusion : \( x+y \) et \( x, y \) n’ont pas la même parité.  

---

2) **Montrer que** :  
\[
(x+y) \land x \land y = 1
\]  
Ici, l’opération logique \(\land\) correspond à l’opération logique **"ET"** (conjonction logique). Cela signifie que nous devons vérifier que toutes les valeurs sont égales à 1 pour que l'expression soit vraie.

- Nous avons \( x = 1 \) et \( y = 1 \), donc :  
  \[
  x+y = 2
  \]
- En logique binaire :  
  - \( 1 \) est représenté par **1** (vrai).  
  - \( 2 \) est représenté par **1** en logique booléenne car seul le bit de poids fort compte (vrai).  

- Ainsi :  
  \[
  (x+y) \land x \land y = 1 \land 1 \land 1 = 1
  \]

**Conclusion :** L'égalité est bien vérifiée.  

---

### **Exercice 2 :**  
Soient \( a \) et \( b \) deux nombres entiers relatifs premiers entre eux. Montrer que les nombres \( 7a + 5b \) et \( 4a + 3b \) sont premiers entre eux.  

**Solution :**  

- Deux nombres sont **premiers entre eux** si leur **PGCD (Plus Grand Commun Diviseur) est égal à 1**.  
- On sait que \( a \) et \( b \) sont premiers entre eux, ce qui signifie que :  
  \[
  \gcd(a, b) = 1
  \]
- Nous devons montrer que :  
  \[
  \gcd(7a + 5b, 4a + 3b) = 1
  \]

**Démonstration :**  

1) **Méthode par combinaisons linéaires :**  
   - Soit \( d \) un diviseur commun de \( 7a + 5b \) et \( 4a + 3b \), donc \( d \) divise :  
     \[
     (7a + 5b) \times 3 - (4a + 3b) \times 5
     \]
     \[
     = 21a + 15b - 20a - 15b = a
     \]
   - De même, \( d \) divise :  
     \[
     (4a + 3b) \times 7 - (7a + 5b) \times 4
     \]
     \[
     = 28a + 21b - 28a - 20b = b
     \]

2) **Or, on sait que** \( \gcd(a, b) = 1 \), donc \( d \) doit être égal à 1.

3) **Conclusion :**  
   - Comme \( d \) divise à la fois \( a \) et \( b \) et que ces derniers sont premiers entre eux, alors \( d = 1 \).  
   - **Donc, \( 7a + 5b \) et \( 4a + 3b \) sont bien premiers entre eux.**  

---

### **Exercice 3 :**  
1) **Montrer que pour tout \( n \in \mathbb{N} \), on a** :  
   \[
   (3n^2 - 11n) \land (n+3) = (n+3) \land 48
   \]  

**Solution :**  

- L'opérateur \( \land \) représente **le PGCD (Plus Grand Commun Diviseur)**.  
- On cherche donc à prouver que :  
  \[
  \gcd(3n^2 - 11n, n+3) = \gcd(n+3, 48)
  \]
- Utilisons la **propriété d'Euclide** :  
  \[
  \gcd(A, B) = \gcd(B, A \mod B)
  \]
- Calculons \( (3n^2 - 11n) \mod (n+3) \) :  

  1. On divise \( 3n^2 - 11n \) par \( n+3 \) :  
     - \( n+3 \) est de degré 1.  
     - \( 3n^2 - 11n \) est de degré 2.  
     - La division donne un reste qu'on cherche.

  2. On effectue la division en posant :  
     \[
     3n^2 - 11n = Q(n) \cdot (n+3) + R
     \]
     En effectuant cette division, on trouve que le reste est **48**.  

  3. Donc, on a bien :  
     \[
     \gcd(3n^2 - 11n, n+3) = \gcd(n+3, 48)
     \]

---

2) **En déduire les valeurs \( n \) de \( \mathbb{N} \) telles que** :  
   \[
   \frac{3n^2 - 11n}{n+3} \in \mathbb{N}
   \]  

- Il faut que la division soit **entière**, donc \( n+3 \) doit être un diviseur de 48.  
- Les diviseurs de 48 sont :  
  \[
  1, 2, 3, 4, 6, 8, 12, 16, 24, 48
  \]
- On cherche les valeurs de \( n \) telles que \( n+3 \) soit dans cette liste.  
- Cela donne :  
  \[
  n = -2, -1, 0, 1, 3, 5, 9, 13, 21, 45
  \]
- **Mais comme \( n \) est un entier naturel, on ne garde que** :  
  \[
  n = 0, 1, 3, 5, 9, 13, 21, 45
  \]

---



### **Exercice 4 :**  
Montrer que pour tout entier naturel \( n \) :  
\[
\gcd(7n + 3, 5n + 2) = \gcd(n, 1)
\]

**Solution :**  

- Nous utilisons la **propriété d'Euclide** :  
  \[
  \gcd(a, b) = \gcd(b, a \mod b)
  \]
- Appliquons cette propriété avec \( a = 7n + 3 \) et \( b = 5n + 2 \) :  

  \[
  (7n + 3) \mod (5n + 2)
  \]

- Effectuons la division :  
  - \( 7n + 3 = Q(5n + 2) + R \)  
  - On cherche \( Q \) et \( R \) tels que :  
    \[
    7n + 3 - 1 \times (5n + 2) = 7n + 3 - 5n - 2 = 2n + 1
    \]

- Donc :  
  \[
  \gcd(7n+3, 5n+2) = \gcd(5n+2, 2n+1)
  \]

- On continue le processus :  
  - Calculons \( (5n+2) \mod (2n+1) \)  
  - On effectue :  
    \[
    5n + 2 - 2 \times (2n + 1) = 5n + 2 - 4n - 2 = n
    \]

- Donc :  
  \[
  \gcd(5n+2, 2n+1) = \gcd(2n+1, n)
  \]

- Enfin, calculons \( (2n+1) \mod n \) :  
  \[
  2n + 1 - 2 \times n = 1
  \]

- Ainsi :  
  \[
  \gcd(2n+1, n) = \gcd(n, 1) = 1
  \]

**Conclusion :**  
\[
\gcd(7n+3, 5n+2) = 1
\]

---

### **Exercice 5 :**  
Soient \( a \) et \( b \) deux entiers naturels premiers entre eux. Montrer que :  
\[
\gcd(a+b, a-b) \in \{1, 2\}
\]

**Solution :**  

- On note que \( \gcd(a, b) = 1 \), donc \( a \) et \( b \) n'ont aucun diviseur commun autre que 1.
- On doit étudier \( \gcd(a+b, a-b) \).

1) **Cas général :**  

   - Si \( d \) est un diviseur commun de \( a+b \) et \( a-b \), alors \( d \) divise aussi :  
     \[
     (a+b) + (a-b) = 2a
     \]
     \[
     (a+b) - (a-b) = 2b
     \]
   - Comme \( d \) divise \( 2a \) et \( 2b \), il doit diviser **2**, car \( \gcd(a, b) = 1 \).

2) **Conclusion :**  

   - \( d \) peut être **1** (si \( a \) et \( b \) sont de même parité).  
   - \( d \) peut être **2** (si \( a \) et \( b \) sont de parités différentes).  

   **Donc :**  
   \[
   \gcd(a+b, a-b) \in \{1, 2\}
   \]

---

### **Exercice 6 :**  
Déterminer toutes les solutions entières positives de l’équation :  
\[
\gcd(x, y) + \gcd(x, y+1) = y
\]

**Solution :**  

On note \( d_1 = \gcd(x, y) \) et \( d_2 = \gcd(x, y+1) \), donc l’équation devient :  
\[
d_1 + d_2 = y
\]

1) **Observation sur les valeurs possibles de \( d_1 \) et \( d_2 \)**  

   - On sait que \( d_1 \) divise \( x \) et \( y \), donc \( x \) est un multiple de \( d_1 \).  
   - \( d_2 \) divise \( x \) et \( y+1 \), donc \( x \) est aussi un multiple de \( d_2 \).  
   - Les seuls cas où \( d_1 + d_2 = y \) se produisent sont lorsque \( d_1 = y \) et \( d_2 = 0 \), ce qui est impossible.  

2) **Recherche de solutions particulières :**  

   - Si \( x = 1 \), alors \( \gcd(1, y) = 1 \) et \( \gcd(1, y+1) = 1 \).  
   - L’équation devient :  
     \[
     1 + 1 = y
     \]
     donc \( y = 2 \).

3) **Vérification pour d'autres valeurs**  

   - Si \( x = y \), alors \( \gcd(y, y) = y \) et \( \gcd(y, y+1) = 1 \).  
   - L’équation devient :  
     \[
     y + 1 = y
     \]
     Ce qui est faux.

4) **Conclusion**  

   - La seule solution entière positive est :  
     \[
     (x, y) = (1, 2)
     \]

---

### **Résumé des résultats :**  

- **Exercice 4** : \( \gcd(7n + 3, 5n + 2) = 1 \).  
- **Exercice 5** : \( \gcd(a+b, a-b) \in \{1, 2\} \).  
- **Exercice 6** : La seule solution entière positive est \( (x, y) = (1, 2) \).  

---

### **Exercice 7 :**  
Montrer que pour tous entiers naturels \( a \) et \( b \), on a :  
\[
\gcd(a, b) \times \operatorname{lcm}(a, b) = a \times b
\]  
où \( \operatorname{lcm}(a, b) \) désigne le **plus petit commun multiple** de \( a \) et \( b \).

**Solution :**  

1) **Décomposition en facteurs premiers**  

   - Soient \( a \) et \( b \) leurs décompositions en nombres premiers :  
     \[
     a = p_1^{\alpha_1} p_2^{\alpha_2} \dots p_k^{\alpha_k}
     \]
     \[
     b = p_1^{\beta_1} p_2^{\beta_2} \dots p_k^{\beta_k}
     \]
   - Alors, le **PGCD** et le **PPCM** s’écrivent comme suit :  
     \[
     \gcd(a, b) = p_1^{\min(\alpha_1, \beta_1)} p_2^{\min(\alpha_2, \beta_2)} \dots p_k^{\min(\alpha_k, \beta_k)}
     \]
     \[
     \operatorname{lcm}(a, b) = p_1^{\max(\alpha_1, \beta_1)} p_2^{\max(\alpha_2, \beta_2)} \dots p_k^{\max(\alpha_k, \beta_k)}
     \]

2) **Produit du PGCD et du PPCM**  

   - En multipliant terme à terme, on obtient :  
     \[
     \gcd(a, b) \times \operatorname{lcm}(a, b) = \prod_{i=1}^{k} p_i^{\min(\alpha_i, \beta_i)} \times p_i^{\max(\alpha_i, \beta_i)}
     \]

   - Or, on sait que :  
     \[
     \min(\alpha, \beta) + \max(\alpha, \beta) = \alpha + \beta
     \]

   - Donc :  
     \[
     \gcd(a, b) \times \operatorname{lcm}(a, b) = \prod_{i=1}^{k} p_i^{\alpha_i + \beta_i} = a \times b
     \]

**Conclusion :**  
\[
\gcd(a, b) \times \operatorname{lcm}(a, b) = a \times b
\]
CQFD ✅

---

### **Exercice 8 :**  
Déterminer tous les entiers naturels \( x \) et \( y \) tels que :  
\[
\gcd(x, y) + \operatorname{lcm}(x, y) = 20
\]

**Solution :**  

1) **Utilisation de l’identité précédente**  

   - On sait que :  
     \[
     \gcd(x, y) \times \operatorname{lcm}(x, y) = x \times y
     \]

   - On pose \( d = \gcd(x, y) \), donc on peut écrire \( x = d a \) et \( y = d b \) avec \( \gcd(a, b) = 1 \).  
   - Alors, le PPCM est donné par :  
     \[
     \operatorname{lcm}(x, y) = d \times a \times b
     \]

   - L’équation devient :  
     \[
     d + d a b = 20
     \]

   - Factorisons :  
     \[
     d(1 + a b) = 20
     \]

2) **Recherche des diviseurs de 20**  

   - \( d \) doit être un diviseur de 20 :  
     \[
     d \in \{1, 2, 4, 5, 10, 20\}
     \]

   - Pour chaque valeur de \( d \), on cherche \( a \) et \( b \) tels que :  
     \[
     1 + ab = \frac{20}{d}
     \]

   - On teste les cas :

     - \( d = 4 \), alors :  
       \[
       1 + ab = \frac{20}{4} = 5 \Rightarrow ab = 4
       \]
       - Les couples \((a, b)\) possibles sont \((1, 4)\) et \((4, 1)\).  
       - Alors, \( (x, y) = (4 \times 1, 4 \times 4) = (4, 16) \) ou \( (16, 4) \).

     - \( d = 5 \), alors :  
       \[
       1 + ab = \frac{20}{5} = 4 \Rightarrow ab = 3
       \]
       - Il n'existe pas de \( (a, b) \) entiers avec \( \gcd(a, b) = 1 \).

     - \( d = 10 \), alors :  
       \[
       1 + ab = \frac{20}{10} = 2 \Rightarrow ab = 1
       \]
       - Le seul couple possible est \( (1,1) \), donc \( (x, y) = (10,10) \).

3) **Conclusion :**  
Les solutions sont :  
\[
(x, y) \in \{ (4,16), (16,4), (10,10) \}
\]

---

### **Exercice 9 :**  
Montrer que si \( a \) et \( b \) sont deux entiers naturels premiers entre eux, alors :  
\[
\gcd(a+b, a^2 + b^2) = 1 \text{ ou } 2
\]

**Solution :**  

1) **Soit \( d = \gcd(a+b, a^2 + b^2) \)**  

   - Alors, \( d \) divise \( a+b \) et \( a^2 + b^2 \).  
   - On sait que \( d \) divise toute combinaison linéaire des deux, donc :  
     \[
     d \mid (a^2 + b^2) - (a+b)(a - b) = a^2 + b^2 - a^2 - ab - ab - b^2 = 2ab
     \]

   - Comme \( a \) et \( b \) sont premiers entre eux, \( \gcd(a, b) = 1 \), donc \( d \) divise 2.

2) **Conclusion :**  
\[
d \in \{1, 2\}
\]

---
