# **ZSAD – Architektura Systemu**

## **1. Struktura systemu**  

System **ZSAD** jest **zdecentralizowaną siecią fizycznych węzłów**, które działają według jednolitego kodu i nie posiadają żadnych dodatkowych modułów spoza głównej implementacji.  
Wszystkie decyzje są podejmowane **kolektywnie**, a ostateczny wybór należy do jednego węzła, tymczasowo wybranego jako **Tyran**.  

---

## **2. Struktura węzła**  

Każdy węzeł składa się z następujących modułów:  

### **A) Moduł komunikacyjny**  
- Obsługuje **szyfrowaną komunikację** między węzłami.  
- Wspiera **sieć mesh** dla redundancji połączeń.  
- Używa **kryptografii asymetrycznej** do weryfikacji tożsamości węzłów.  
- Przechowuje **tymczasowe klucze sesyjne** dla szybkiej wymiany danych.  

### **B) Moduł podejmowania decyzji**  
- Wykonuje **lokalną analizę** dostępnych danych.  
- Przyjmuje decyzje od innych węzłów i **konsoliduje je w ramach mechanizmu Tyrana**.  
- Zawiera zestaw **algorytmów analizy strategicznej**, minimalizacji strat i optymalizacji reakcji.  

### **C) Moduł diagnostyczny**  
- Monitoruje **stan własny i sąsiadujących węzłów**.  
- Wykrywa **nienaturalne wzorce zachowań**, które mogą wskazywać na awarię lub atak.  
- Raportuje wyniki do sieci w przypadku podejrzenia problemów.  

### **D) Moduł zabezpieczeń**  
- Odpowiada za **integralność kodu** i zapewnia, że kod węzła nie został zmodyfikowany.  
- Blokuje **nieautoryzowane próby ingerencji w oprogramowanie**.  
- Przeprowadza **cykliczną weryfikację poprawności działania**.  

---

## **3. Struktura komunikacji między węzłami**  

### **A) Mechanizmy wymiany danych**  
- Komunikacja oparta na **asynchronicznych pakietach wiadomości**, ograniczonych do **minimalnego** zbioru danych.  
- Każda wiadomość zawiera:  
  - **ID nadawcy** (zaszyfrowane).  
  - **Losowy numer sesji**, aby uniknąć ataków powtórzeniowych.  
  - **Skrót wiadomości (hash)** zabezpieczony kluczem prywatnym.  

### **B) Proces podejmowania decyzji przez Tyrana**  
1. Węzły **przesyłają swoje analizy** do Tyrana.  
2. Tyran **agreguje dane**, stosuje mechanizmy **wykrywania fałszywych wyników** i wybiera optymalną decyzję.  
3. Tyran przesyła decyzję do **sieci kontrolnej**, gdzie inne węzły dokonują jej weryfikacji.  
4. Po zatwierdzeniu decyzji, **zostaje ona wykonana** przez system.  

### **C) Mechanizm wyboru Tyrana**  
- Proces wyboru Tyrana bazuje na **algorytmie Tyrana**, który:  
  - **Losowo wybiera kandydata**, eliminując możliwość przewidywania.  
  - Wymaga **zatwierdzenia przez inne węzły**, aby uniknąć ataków.  
  - Gwarantuje **tymczasowość roli** – Tyran zmienia się cyklicznie.  

---

## **4. Struktura hierarchiczna systemu**  

System nie posiada **centralnego zarządzania**, ale operuje w **strukturze adaptacyjnej**:  

1. **Węzły podstawowe** – główna warstwa systemu, odpowiedzialna za analizę i decyzje.  
2. **Węzły kontrolne** – pełnią funkcję monitorującą, sprawdzają poprawność decyzji i wykrywają anomalie.  
3. **Tyran** – pełni funkcję ostatecznego decydenta na czas jednej operacji.  

Każda warstwa **współpracuje dynamicznie**, co oznacza, że role są zmienne i **dowolny węzeł może przejąć inną funkcję** w zależności od potrzeb.  

---

## **5. Skalowalność i optymalizacja**  

System został zaprojektowany tak, aby był **łatwo skalowalny**:  

### **A) Dynamiczne zarządzanie węzłami**  
- Każdy węzeł posiada algorytmy **samoorganizacji**, pozwalające dostosować się do zmieniającej się liczby jednostek.  
- Brak **stałych połączeń między węzłami** – struktura dostosowuje się dynamicznie.  

### **B) Optymalizacja ruchu w sieci**  
- Węzły **nie przesyłają zbędnych danych**, tylko **podsumowania** i wyniki analiz.  
- System stosuje **kompresję danych** i **eliminację redundancji**, aby zmniejszyć zużycie zasobów.  

---

## **6. Zasady bezpieczeństwa**  

1. **Każdy węzeł działa według tego samego kodu** – brak dodatkowych komponentów zwiększa odporność na modyfikacje.  
2. **Weryfikacja każdej decyzji przez kilka innych węzłów** – unikanie manipulacji i fałszywych wyników.  
3. **Brak stałego centrum dowodzenia** – eliminacja głównego punktu awarii.  
4. **Tyran nigdy nie działa samodzielnie** – decyzje są kolektywne.  
5. **Szyfrowanie asymetryczne** – każda transmisja w systemie jest bezpieczna.  
6. **Dynamiczna zmiana kluczy sesyjnych** – każda operacja generuje nowe klucze, co utrudnia ataki.  

---

## **7. Podsumowanie**  

System **ZSAD** jest w pełni **zdecentralizowaną, autonomiczną siecią** podejmującą decyzje w sposób **kolektywny i dynamiczny**, przy zachowaniu **wysokiego poziomu bezpieczeństwa, odporności na ataki i zdolności adaptacyjnych**.  

### **Kluczowe cechy architektury:**  
- **Brak centralnego sterowania** – węzły działają samodzielnie, ale w koordynacji.  
- **Każdy węzeł jest identyczny** – jednolity kod eliminuje manipulacje.  
- **Kolektywne podejmowanie decyzji** – wybór Tyrana w sposób dynamiczny.  
- **Zaawansowane mechanizmy kryptograficzne** – gwarancja integralności i autoryzacji.  
- **Optymalizacja ruchu w sieci** – minimalizacja wymiany danych i redundancji.  
- **Odporność na manipulację** – system dynamicznie wykrywa fałszywe decyzje i anomalie.  

System **ZSAD** łączy **nowoczesne technologie** z **autonomiczną analizą strategiczną**, tworząc sieć, która **może działać bez zewnętrznej kontroli, a jednocześnie jest odporna na przejęcie i awarie**.
