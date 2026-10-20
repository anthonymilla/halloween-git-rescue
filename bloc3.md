# 🚀 Bloc 3: Viatge Temporal, Exorcisme del Codi i Publicació Remota

### Acció 3.11: Registre del commit infectat de l'esperit maligne
**Explicació tècnica:** Es simula la corrupció del programador desaparegut afegint una excepció espectral maliciosa a l'historial per registrar aquest estat defectuós.
```bash
git add main.js
git commit -m "feat: unhandled spectral exception"
```
![Captura del commit infectat](captura11.png)

---

### Acció 3.12: Inspecció de la diferència textual exacta de la corrupció
**Explicació tècnica:** S'utilitza l'ordre `git diff` per analitzar textualment el codi nociu introduït per l'esperit en contrast amb el darrer commit segur de la línia de temps (`HEAD~1`).
```bash
git diff HEAD~1 HEAD
```
![Captura de la diferència amb git diff](captura12.png)

---

### Acció 3.13: Reversió temporal i eliminació destructiva (Exorcisme)
**Explicació tècnica:** S'executa un comandament de restauració severa en mode forçat (`--hard`) per desplaçar el punter enrere, esborrar el commit infectat de l'historial permanentment i netejar l'espai de treball.
```bash
git reset --hard HEAD~1
```
![Captura de l'exorcisme amb git reset](captura13.png)

---

### Acció 3.14: Visualització gràfica de la topologia final purificada
**Explicació tècnica:** Es genera el diagrama gràfic directe a la terminal de l'arbre de Git per assegurar que el flux de branques i fusions és net i lliure de corrupció.
```bash
git log --oneline --graph --all
```
![Captura de la topologia en arbre](captura14.png)

---

### Acció 3.15: Creació i vinculació del repositori a GitHub (Publicació remota)
**Explicació tècnica:** Es vincula el repositori local purificat amb el servidor remot públic allotjat a GitHub i es pugen totes les dades i línies temporals de seguretat històriques.
```bash
git remote add origin https://github.com
git push -u origin master --all
```
![Captura de la pujada final a GitHub](captura15_1.png)
![Captura de la pujada final a GitHub](captura15_2.png)