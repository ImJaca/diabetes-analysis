### Uruchomienie kontenera (terminal)

W folderze głównym projektu:

docker compose -f docker/docker-compose.yml up --build

---

###  Zatrzymanie kontenera

docker compose -f docker/docker-compose.yml down

---

##  Uruchamianie w VS Code

### Terminal w VS Code

``Zainstaluj rozszerzenie **Dev Containers**``

1. Otwórz projekt w VS Code
2. Otwórz terminal (Ctrl + ~)
3. Wpisz: docker compose -f docker/docker-compose.yml up --build
4. Ctrl + Shift + P
5. Wybierz: Dev Containers: Reopen in Container

---