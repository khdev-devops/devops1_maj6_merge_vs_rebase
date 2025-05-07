# Delövning 2: Rebase

I denna delövning ska du öva på att använda `git rebase` för att integrera dina ändringar ovanpå en annan branch. Du kommer att arbeta i en branch som heter `rebase-demo`, och när du är klar ska du rebasea dina ändringar in i den branchen.

## Steg

1. Skapa en ny branch från `main`:
   ```
   git checkout main
   git pull
   git checkout -b ditt-namn-rebase
   ```

2. Ändra i denna fil genom att lägga till ditt namn i listan under "Deltagarlista".

3. Gör en commit:
   ```
   git add rebase.md
   git commit -m "Lade till mitt namn i rebase.md"
   ```

4. Byt till `rebase-demo`-branchen och uppdatera den:
   ```
   git checkout rebase-demo
   git pull
   ```

5. Rebasea din branch på `rebase-demo`:
   ```
   git checkout ditt-namn-rebase
   git rebase rebase-demo
   ```

6. Byt till `rebase-demo` och mergea din rebased branch:
   ```
   git checkout rebase-demo
   git merge ditt-namn-rebase
   git push
   ```

## Deltagarlista

- [Lägg till ditt namn här]
- Jonas
- Jiadai
- Shaheera
- Detelina
-Gustaf

Klas was here as well!

## Klar?

När läraren visat hur git historiken ser ut med alla ändringar är övningen avslutad. Tack!