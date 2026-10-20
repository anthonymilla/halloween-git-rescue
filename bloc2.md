# 👻 Bloc 2: Les Branques del Més Enllà i Resolució del Conflicte

### Acció 3.6: Creació de dues branques noves (feature-nightmare i feature-sanctuary)
**Explicació tècnica:** Es creen dues línies temporals de desenvolupament paral·lel basades en l'últim commit de `master`. Es defensa una topologia divergent per garantir que les branques experimentals no corrompin la branca activa de producció.
```bash
git branch feature-nightmare
git branch feature-sanctuary
```
![Captura de la creació de branques](captura6.png)

---

### Acció 3.7: Desplaçament i modificació a la branca feature-nightmare
**Explicació tècnica:** Ens desplacem a la branca de la dimensió fosca utilitzant `checkout`. Es modifica la lògica del fitxer `main.js` per injectar el codi de la corrupció i es crea un nou commit.
```bash
git checkout feature-nightmare
git add main.js
git commit -m "fix: injecting dark dimension logic"
```
![Captura del treball a feature-nightmare](captura7_1.png)
![Captura del treball a feature-nightmare](captura7_2.png)

---

### Acció 3.8: Desplaçament i modificació a la branca feature-sanctuary
**Explicació tècnica:** Canviem a la línia de protecció del santuari. Es modifica la mateixa línia de codi del fitxer `main.js` amb el codi de defensa alternatiu i es registra el canvi.
```bash
git checkout feature-sanctuary
git add main.js
git commit -m "feat: alternative sanctuary protection matrix"
```
![Captura del treball a feature-sanctuary](captura8.png)

---

### Acció 3.9: Retorn a la branca principal i intents d'integració
**Explicació tècnica:** Es torna a la branca principal `master`. La primera integració es realitza correctament. En intentar integrar la segona branca, el sistema detecta canvis simultanis a la mateixa línia, provocant una col·lisió de línies temporals (conflicte).
```bash
git checkout master
git merge feature-nightmare
git merge feature-sanctuary
```
![Captura del conflicte de fusió](captura9.png)

---

### Acció 3.10: Anàlisi, depuració manual de marques i commit de fusió final
**Explicació tècnica:** S'obre el fitxer afectat a VS Code, s'eliminen manualment les marques de Git (`<<<<<<<`, `=======`, `>>>>>>>`) i es tria la combinació de codi definitiva per salvar el servidor, finalitzant el procés amb el commit de fusió.
```bash
git add main.js
git commit -m "merge: resolving timeline collision and saving core server"
```
![Captura del commit de fusió](captura10.png)