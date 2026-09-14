### Documentation officielle uv
https://docs.astral.sh/uv/getting-started/installation/

### Pour installer uv 
```bash 
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```
### Pour lire pyproject.toml et uv.lock (télécharge et recrée le.venv)
```bash 
uv sync 
```
### Pour lancer Jupyter Lab en utilisant cet environnement
```bash 
uv run jupyter lab 
```
### Pour activer l'environnement virtuel
```bash 
.venv\Scripts\activate
```
### Si message d’erreur “Impossible de charger le fichier…. 
```bash 
Set-ExecutionPolicy Unrestricted
```
### Ajouter une librairie
```bash 
uv add <nom de la librairie>
```
### Désinstaller une dépendance
```bash 
uv remove <nom de la librairie>
```
### Passer de requirements.txt à uv
```bash 
uv add -r requirements.txt
```
### Mettre à jour les dépendances
```bash 
uv lock --upgrade
```