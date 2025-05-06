# Delövning 1: Merge

 I denna delövning ska du öva på att använda `git merge` för att integrera ändringar från en egen branch till huvudbranchen. Du kommer att arbeta i en branch som heter `merge-demo`, och när du är klar ska du mergea dina ändringar in i den branchen.

## Steg

1. Skapa en ny branch från `main`:
   ```
   git checkout main
   git pull
   git checkout -b ditt-namn-merge
   ```

2. Ändra i denna fil genom att lägga till ditt namn i listan under "Deltagarlista".

3. Gör en commit:
   ```
   git add merge.md
   git commit -m "Lade till mitt namn i merge.md"
   ```

4. Byt till `merge-demo`-branchen och uppdatera den:
   ```
   git checkout merge-demo
   git pull
   ```

5. Mergea din branch in i `merge-demo`:
   ```
   git merge ditt-namn-merge
   ```

6. Pusha upp ändringarna:
   ```
   git push
   ```

## Deltagarlista

- [Lägg till ditt namn här]
Shaheera
- Jonas
- Gustaf
Detelina
Detelina

## Klar?

När läraren visat hur git historiken ser ut med alla ändringar kan du gå vidare till [nästa delövning](./rebase.md).