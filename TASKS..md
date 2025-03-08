# Wymagania funkcjonalne:

> - System powinien identyfikować zagrożenia na podstawie analizy danych, takich jak obrazy satelitarne, dane radarowe i sygnały elektroniczne.
> - System będzie analizował sytuacje przy użyciu sztucznej inteligencji i podejmował decyzje całkowicie autonomicznie, bez możliwości ingerencji zewnętrznej.
> - Każdy węzeł systemu będzie zawierał cząstkowy obraz sytuacji i będzie się komunikował z pozostałymi węzłami w sposób zdecentralizowany.
> - System w razie potrzeby aktywuje środki obronne i steruje nimi, bazując na dostępnych danych oraz algorytmach optymalizacji decyzji.
> - System nie będzie wymagał ingerencji ludzkiej ani nie będzie możliwy do sterowania przez operatora, eliminując możliwość przejęcia przez sabotażystów.
> - Węzły systemu będą wyposażone w mechanizmy autodiagnostyki oraz autonomicznej naprawy, aby minimalizować skutki uszkodzeń.
> - Sieć systemu będzie adaptacyjna, zdolna do reorganizacji w czasie rzeczywistym, tak aby system z niemalże zerowym opóźnieniem odzyskiwał stabilność nawet po utracie znaczącej liczby węzłów.

# Wymagania niefunkcjonalne:

> - Czas reakcji systemu powinien wynosić nie więcej niż 1 sekundę.
> - Komunikacja między węzłami będzie zaszyfrowana w celu zapewnienia bezpieczeństwa transmisji danych.
> - Sztuczna inteligencja użyta w systemie zostanie wytrenowana do wykrywania fałszywych sygnałów i niepodejmowania działań na ich podstawie.
> - System będzie zdolny do adaptacyjnej analizy podejmowanych decyzji w czasie rzeczywistym, optymalizując swoje działanie na podstawie dynamicznych warunków operacyjnych.
> - Architektura systemu będzie odporna na ataki cybernetyczne oraz fizyczne, wykorzystując redundancję oraz mechanizmy rozproszonej ochrony.
> - Sieć systemu powinna automatycznie dostosowywać swoją strukturę do uszkodzeń i rekonfigurować się w celu zapewnienia ciągłości działania nawet w przypadku awarii wielu węzłów.
	
# Epiki
> - **Epik 1** Projektowanie architektury systemu
>   - Task 1: Wymagania systemowe
>   - Task 2: Wybór technologii
>   - Task 3: Model komunikacji
>   - Task 4: System węzłów
> - **Epik 2** Implementacja zdecentralizowanej sieci komunikacyjnej
>   - Task 1: Protokół wymiany danych     
>   - Task 2: Szyfrowanie i anonimizacja
>   - Task 3: Testy
>   - Task 4: Optymalizacja
> - **Epik 3** Integracja AI do analizy zagrożeń
>   - Task 1: Zdefiniowanie scenariuszy
>   - Task 2: Trenowanie AI
>   - Task 3: Mechanizmy decyzyjne
>   - Task 4: Testowanie i kalibracja
> - **Epik 4** System sterowania uzbrojeniem
>   - Task 1: Algorytmy sterowania
>   - Task 2: Integracja AI
>   - Task 3: Symulacje i testy
>   - Task 4: Weryfikacja poprawności działania
> - **Epik 5** Bezpieczeństwo systemu
>   - Task 1: Symulacje ataków
>   - Task 2: Testy infrastruktury
>   - Task 3: Testy zabezpieczeń
>   - Task 4: Dokumentacja

## User Stories

> - **Epik 1** Projektowanie architektury systemu
>   - **Task 1:** Jako strateg wojskowy, chcę jasno określić wymagania systemowe, aby mieć pewność, że system spełnia nasze potrzeby operacyjne i może działać w każdych warunkach bojowych.
>   - **Task 2:** Jako operator systemu obronnego, chcę, aby wykorzystane technologie były nowoczesne, skalowalne i odporne na ataki, aby zapewnić maksymalną niezawodność systemu.
>   - **Task 3:** Jako dowódca, chcę mieć pewność, że komunikacja między węzłami odbywa się bez opóźnień i ryzyka przejęcia przez wroga, aby decyzje były podejmowane w czasie rzeczywistym.
>   - **Task 4:** Jako inżynier wojskowy, chcę, aby system składał się z niezależnych węzłów, które mogą przejąć zadania w przypadku awarii innych jednostek, aby zapewnić ciągłość działania systemu.
> - **Epik 2** Implementacja zdecentralizowanej sieci komunikacyjnej
>   - **Task 1:** Jako oficer odpowiedzialny za cyberbezpieczeństwo, chcę, aby protokół wymiany danych był zoptymalizowany pod kątem szybkości i odporności na przechwycenie, aby system mógł działać nawet w warunkach wojny elektronicznej.
>   - **Task 2:** Jako operator systemu, chcę mieć pewność, że wszystkie dane są szyfrowane i nie można ich powiązać z konkretnymi węzłami, aby przeciwnik nie mógł wykryć i zneutralizować struktury sieci.
>   - **Task 3:** Jako analityk wojskowy, chcę by były przeprowadzone testy penetracyjne systemu, aby upewnić się, że nie ma luk umożliwiających przejęcie kontroli przez wroga.
>   - **Task 4:** Jako operator systemu, chcę, aby sieć działała z minimalnym zużyciem zasobów, ale przy zachowaniu maksymalnej przepustowości, aby operacje nie były ograniczane przez opóźnienia.
> - **Epik 3** Integracja AI do analizy zagrożeń
>   - **Task 1:** Jako sztab wojskowy, chcemy określić pełną listę zagrożeń, które system powinien wykrywać, aby AI mogła odpowiednio reagować na wszystkie potencjalne ataki.
>   - **Task 2:** Jako inżynier systemów obronnych, chcę, aby AI była trenowana na rzeczywistych przypadkach zagrożeń, aby podejmowała trafne decyzje i nie generowała fałszywych alarmów.
>   - **Task 3:** Jako operator wojskowy, chcę, aby AI mogła autonomicznie podejmować decyzje.
>   - **Task 4:** Jako dowódca sił obronnych, chcę, aby system był testowany w różnych warunkach operacyjnych, aby mieć pewność, że AI podejmuje trafne decyzje w sytuacjach krytycznych.
> - **Epik 4** System sterowania uzbrojeniem
>   - **Task 1:** Jako strateg wojskowy, chcę, aby algorytmy sterowania uzbrojeniem były zoptymalizowane pod kątem precyzyjnego trafienia w cel i omijania obrony przeciwnika.
>   - **Task 2:** Jako operator systemu rakietowego, chcę, aby AI mogła dynamicznie zmieniać trajektorię rakiet w zależności od sytuacji na polu walki, aby zwiększyć skuteczność ataku.
>   - **Task 3:** Jako analityk wojskowy, chcę by przeprowadzono symulacje ataków i kontrataków, aby sprawdzić, jak system sterowania uzbrojeniem zachowuje się w różnych scenariuszach.
>   - **Task 4:** Jako dowódca sił rakietowych, chcę, aby system był gruntownie testowany pod kątem poprawności działania, aby uniknąć przypadkowej aktywacji lub błędnej identyfikacji celu.
> - **Epik 5** Bezpieczeństwo systemu
>   - **Task 1:** Jako ekspert ds. cyberbezpieczeństwa, chcę aby przeprowadzono realistyczne symulacje ataków na system, aby upewnić się, że jest odporny na przejęcie.
>   - **Task 2:**  Jako inżynier wojskowy, chcę by sprawdzono, jak system zachowa się w przypadku uszkodzenia fizycznego węzłów, aby mieć pewność, że system działa nawet przy częściowej awarii infrastruktury.infrastruktury
>   - **Task 3:** Jako dowódca jednostki odpowiedzialnej za system, chcę mieć pewność, że nikt niepowołany nie uzyska dostępu do systemu i nie zmieni jego decyzji.
>   - **Task 4:** Jako szkoleniowiec wojskowy, chcę mieć dostęp do jasnej dokumentacji systemu, aby móc szybko szkolić nowych operatorów i zapobiec błędom w jego użytkowaniu.
