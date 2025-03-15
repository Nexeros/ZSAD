# **ZSAD – Odporność na Awarie i Ataki w Sieci Fizycznych Węzłów**

System **ZSAD** oparty na fizycznych węzłach musi zapewniać **maksymalne bezpieczeństwo, adaptacyjność i skalowalność**. Węzły są identyczne i posiadają ten sam kod. Decyzje są podejmowane kolektywnie przez wybranego **Tyrana**, który zbiera informacje od innych węzłów i dokonuje ostatecznych wyborów.  

---

## **1. Wykrywanie uszkodzonych węzłów**  

Każdy węzeł posiada **moduł diagnostyczny**, który monitoruje jego pracę oraz stan sąsiadujących jednostek. **Żaden węzeł nie może samodzielnie stwierdzić awarii innego węzła** – wymagana jest potwierdzona zgodność z kilkoma innymi węzłami.  

### **A) Mechanizmy wykrywania awarii**  
- **Testy heartbeat** – okresowe sygnały życia do sąsiadujących węzłów.  
- **Losowa kontrola integralności** – testy odpowiedzi na losowe żądania.  
- **Weryfikacja decyzji** – porównanie wyników decyzji węzła z innymi.  
- **Monitorowanie sygnatury pracy** – analiza zmian w wydajności i czasie odpowiedzi.  

### **B) Proces zgłaszania awarii**  
1. Węzeł A wykrywa problem z węzłem B.  
2. Węzeł A pyta kilka innych losowych węzłów o ich obserwacje.  
3. Jeśli większość potwierdzi problem, węzeł B jest oznaczany jako uszkodzony.  
4. Informacja o awarii zostaje rozesłana do całej sieci.  

---

## **2. Mechanizmy radzenia sobie z awariami węzłów**  

### **A) Dynamiczne przekierowanie ruchu**  
- Węzły **nie tworzą sztywnej hierarchii** – po awarii jeden z nich przejmuje jego zadania.  
- Każdy węzeł posiada kilka alternatywnych ścieżek komunikacji.  

### **B) Awaryjne wybieranie nowego Tyrana**  
- Jeśli Tyran ulegnie awarii, system wybiera nowego poprzez **losowanie liczb hashujących**.  
- Proces jest zdecentralizowany i nie wymaga centralnego nadzoru.  

### **C) Minimalizacja wpływu pojedynczych awarii**  
- Węzły **nie przechowują pełnych kopii danych**.  
- Decyzje **nie są zależne od pojedynczego węzła**.  

---

## **3. Odporność na ataki i manipulacje**  

### **A) Mechanizmy wykrywania ataków**  
- **Analiza wzorców ruchu** – nietypowe wzrosty aktywności sygnalizują atak.  
- **Weryfikacja sygnatur** – wszystkie dane są podpisywane cyfrowo.  
- **Losowe testy spójności** – weryfikacja poprawności operacji.  

### **B) Ochrona przed przejęciem Tyrana**  
- **Tyran nie podejmuje decyzji samodzielnie** – jego wybory są zatwierdzane przez inne węzły.  
- Jeśli Tyran działa podejrzanie, może zostać usunięty i zastąpiony nowym.  

### **C) Odporność na fałszywe węzły (atak Sybil)**  
- Nowe węzły **nie mogą dołączać do sieci bez autoryzacji**.  
- Dopiero po przejściu testów mogą uczestniczyć w podejmowaniu decyzji.  

---

## **4. Mechanizmy adaptacyjne**  

### **A) Dynamiczna zmiana algorytmów**  
- System może **modyfikować część swojego kodu**, aby utrudnić ataki.  
- Algorytm wyboru Tyrana może się zmieniać w sposób losowy.  

### **B) Inteligentna reakcja na ataki**  
- Wykrycie ataku może powodować **tymczasowe zamrożenie operacji**.  
- Węzły mogą przechodzić w **tryb izolacji**, ograniczając dostęp atakujących.  

---

## **Podsumowanie**  

### **Odporność na awarie:**  
- Węzły **monitorują się nawzajem** i wspólnie oceniają awarie.  
- **Automatyczne przekierowanie ruchu** w razie awarii.  
- **Dynamiczny wybór nowego Tyrana**, brak centralnego punktu awarii.  

### **Odporność na ataki:**  
- **Decyzje są kolektywne**, eliminując możliwość przejęcia systemu.  
- **Każde zapytanie i decyzja są podpisywane cyfrowo**.  
- System **automatycznie zmienia algorytmy**, utrudniając przewidywanie jego zachowania.  

### **Odporność na manipulację danymi:**  
- **Weryfikacja integralności decyzji** zapobiega fałszowaniu informacji.  
- **Losowe testy** zabezpieczają przed próbami manipulacji.  
- **Brak pojedynczego punktu kontroli** – Tyran zawsze działa pod nadzorem innych węzłów.  

---

System **ZSAD**, oparty na fizycznych węzłach, zapewnia **maksymalną odporność na ataki i awarie** poprzez **decentralizację, dynamiczne przekierowanie ruchu oraz kolektywne podejmowanie decyzji**. Każdy węzeł działa **niezależnie, ale w harmonii z innymi**, tworząc **sieć praktycznie niemożliwą do zniszczenia lub przejęcia**.
