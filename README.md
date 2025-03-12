# Merge con Manu

## Osito Lulu

```bash
# hacer un commit desde la rama colab
git add .\README.md
git commit -m "1"
```
```bash
# hacer otro commit desde la rama colab
git add .\README.md
git commit -m "2"
```
```bash
# hacer otro commit
git add .\README.md
git commit -m "3"
```

```bash
# hacer un commit desde la rama lider
git add .\README.md
git commit -m "A"
```
```bash
# hacer otro commit desde la rama lider
git add .\README.md
git commit -m "B"
```
```bash
# hacer otro commit
git add .\README.md
git commit -m "C"
```
# Merge rama colaborador
```bash
git checkout master
git merge colaborador
git add .\README.md
git commit -m "Merge listo"
```

# Hacer el merge con la rama líder
```bash
# vamos a la rama main
git checkout main
# cargamos los cambios del colaborador
git pull
# hacemos el merge squash con la rama lider
git merge --squash lider
# solo faltará corregir los conflictos y ya
```