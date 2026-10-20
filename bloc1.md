# 🧙‍♂️ Bloc 1: Invocació del Repositori i Línia Base

### Acció 3.1: Creació del directori i estructura inicial de Git
**Explicació tècnica:** S'ha inicialitzat un repositori buit local de Git per començar el seguiment de versions i reconstruir l'entorn afectat des de zero.
```bash
git init
```
![Captura del comando git init](captura1.png)

---

### Acció 3.2: Configuració del control de versions amb perfil professional
**Explicació tècnica:** S'estableixen les variables de configuració de l'usuari local per identificar formalment l'autor de les accions de recuperació en el registre històric.
```bash
git config user.name "Anthony Milla"
git config user.email "tu_correo@estudiant.com"
```
![Captura de la configuració d'usuari](captura2.png)

---

### Acció 3.3: Generació del fitxer principal de l'aplicació i primer commit
**Explicació tècnica:** Es crea el fitxer de codi base `main.js` per establir el punt de partida de l'aplicació. Posteriorment, s'afegeix a l'àrea de preparació i es consolida el primer commit formal.
```bash
git add main.js
git commit -m "feat: initial formal structure for server environment"
```
![Captura del primer commit](captura3.png)

---

### Acció 3.4: Aplicació de dues modificacions successives per al sistema de seguretat
**Explicació tècnica:** Es realitzen dos canvis seqüencials en el fitxer `main.js` per implementar filtres perimetrals i el cortafocs. Cada modificació es registra per separat mitjançant commits independents.
```bash
git add main.js
git commit -m "feat: implement perimetric security filters"

git add main.js
git commit -m "feat: deploy main server room firewall"
```
![Captura del segon i tercer commit](captura4.png)

---

### Acció 3.5: Consulta de l'historial simplificat en una sola línia
**Explicació tècnica:** S'executa una consulta del registre per comprovar els commits realitzats, verificant que la línia temporal inicial de la branca `master` és totalment estable.
```bash
git log --oneline
```
![Captura de l'historial simplificat](captura5.png)