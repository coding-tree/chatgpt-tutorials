Świetnie, możemy skupić się bardziej na codziennej pracy nad projektem i tym, jak Git pomaga śledzić każdy etap, z naciskiem na użycie odpowiednich komend. Wyobraźmy sobie, że książka to projekt, a Git to Twój pamiętnik, który pomaga Ci zapamiętać każdy krok. Oto jak możesz korzystać z Gita w codziennej pracy nad książką.

---

## **Codzienna praca nad książką z Git**

### **1. Sprawdzanie statusu projektu – `git status`**
(Obrazek dziecka z notatką i listą rzeczy do zrobienia)

Każdego dnia, kiedy siadasz do pracy nad książką, warto zobaczyć, co jest już zrobione, a co jeszcze czeka na zapisanie. Aby sprawdzić, co zmieniło się w Twoim projekcie od ostatniego zapisu, używamy komendy:

```bash
git status
```

Git pokaże Ci, jakie pliki zostały zmienione, a także które z nich jeszcze nie zostały zapisane (commitowane). To jak przeglądanie swojego dziennika, żeby zobaczyć, nad czym pracowałeś wczoraj.

### **2. Sprawdzanie różnic – `git diff`**
(Obrazek z dwiema stronami książki – stara wersja i nowa wersja – z podkreślonymi zmianami)

Zanim zapiszesz zmiany, możesz chcieć zobaczyć, co dokładnie zmieniłeś w swojej książce. Na przykład, co dodałeś do nowego rozdziału. Komenda `git diff` pokaże Ci te różnice:

```bash
git diff
```

Git pokaże, co zostało dodane (zielone), a co usunięte (czerwone). To jak zaznaczanie różnic w dwóch wersjach tego samego tekstu.

### **3. Dodawanie zmian do zapisania – `git add`**
(Obrazek dziecka zbierającego strony książki i wkładającego je do skrzyni)

Kiedy już zobaczysz, co zmieniłeś i jesteś zadowolony, czas dodać te zmiany do Git, aby je później zapisać. Używamy `git add` do zebrania zmian, które chcesz zachować:

```bash
git add nazwa_pliku
```

Możesz dodać jeden konkretny plik, nad którym pracowałeś, albo wszystkie zmiany naraz:

```bash
git add .
```

To jak zbieranie stron, które napisałeś, zanim schowasz je do swojej magicznej skrzyni z wersjami.

### **4. Zapisywanie zmian – `git commit`**
(Obrazek dziecka piszącego w dzienniku: "Dodałem nowy rozdział")

Teraz czas na zapisanie tych zmian. To tak, jakbyś pisał notatkę w swoim dzienniku o tym, co zrobiłeś dzisiaj. W komendzie `git commit` możesz napisać krótką wiadomość, co zmieniłeś:

```bash
git commit -m "Dodałem nowy rozdział o przygodach smoka"
```

Każdy commit to zapisany krok w pracy nad książką. To jak wpis do dziennika, który mówi, co zostało zrobione.

### **5. Historia zmian – `git log`**
(Obrazek kalendarza z wpisami, co zostało zrobione każdego dnia)

Czasem chcesz przypomnieć sobie, co robiłeś w poprzednich dniach. Git może Ci pokazać pełną historię zapisanych zmian za pomocą `git log`. Możesz zobaczyć wszystkie swoje „wpisy do dziennika”:

```bash
git log
```

Dzięki temu wiesz, kiedy dodałeś nowy rozdział lub kiedy poprawiłeś literówki w starym.

### **6. Praca nad różnymi wersjami – `git branch` i `git checkout`**
(Obrazek drzewa z gałęziami – każda gałąź to nowa wersja książki)

Czasem podczas pracy nad książką chcesz wypróbować nowy pomysł, ale nie jesteś pewien, czy jest lepszy od starego. Możesz stworzyć nową **gałąź** (branch), w której będziesz eksperymentować, bez psucia oryginalnej wersji.

Najpierw tworzysz nową gałąź:

```bash
git branch nowa-wersja
```

Potem przechodzisz do niej, aby nad nią pracować:

```bash
git checkout nowa-wersja
```

Teraz jesteś w nowej gałęzi, gdzie możesz pisać nowe rozdziały lub zmieniać zakończenie. Jeśli uznasz, że to była dobra decyzja, możesz połączyć nową wersję z główną książką.

### **7. Łączenie wersji – `git merge`**
(Obrazek dwóch ścieżek, które łączą się w jedną)

Gdy jesteś zadowolony z nowych zmian w alternatywnej gałęzi, możesz wrócić do głównej wersji i połączyć je za pomocą `git merge`. Najpierw wracasz do głównej gałęzi (main):

```bash
git checkout main
```

Następnie łączysz zmiany z alternatywnej gałęzi:

```bash
git merge nowa-wersja
```

Teraz masz jedną wersję książki, która zawiera wszystkie nowe pomysły.

### **8. Codzienna praca zespołowa – `git pull` i `git push`**
(Obrazek kilku dzieci pracujących razem nad książką)

Kiedy pracujesz z innymi nad książką (np. na GitHubie), musisz upewnić się, że masz najnowszą wersję projektu. Zanim zaczniesz pracować, pobierz najnowsze zmiany od swojego zespołu za pomocą `git pull`:

```bash
git pull origin main
```

Kiedy skończysz pracę, możesz wrzucić swoje zmiany do wspólnego repozytorium, aby inni mogli je zobaczyć:

```bash
git push origin main
```

To jak współdzielenie notatek z przyjaciółmi, aby każdy mógł przeczytać, co zmieniłeś.

---

### **Podsumowanie codziennej pracy:**
1. **Sprawdź status**: `git status`
2. **Zobacz, co zmieniłeś**: `git diff`
3. **Dodaj zmiany**: `git add`
4. **Zapisz zmiany**: `git commit`
5. **Sprawdź historię**: `git log`
6. **Pracuj nad różnymi wersjami**: `git branch` i `git checkout`
7. **Łącz wersje**: `git merge`
8. **Pracuj z zespołem**: `git pull` i `git push`

Dzięki tym krokom, Twoja codzienna praca nad książką będzie uporządkowana, a Ty zawsze będziesz wiedział, co dokładnie zostało zrobione!
