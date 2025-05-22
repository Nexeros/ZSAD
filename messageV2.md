# Taski
## **1.** Komponenty wewnętrzne modułu decyzyjnego 
**a)** Zaprogramowanie sub-modułu diagnostycznego
> - komunikacja                                                             **M**
> - logika                                                                  **M**
> - selfcheck                                                               **M**

**b)** Zaprogramowanie sub-modułu silnika analitycznego
> - standaryzacja postaci danych                                            **L**
> - logika                                                                  **XL**
> - selfcheck                                                               **M**

**c)** Zaprogramowanie logiki modułu
> - wybór tyrana                                                            **XL**
> - datatraffic                                                             **L**
> - selfcheck                                                               **M**

**d)** Zaprogramowanie modułów AI
> - zaprogramowanie sub-modułu pionka                                       **XXL**
> - datatraffic dla bazy danych                                             **L**
> - unifikacja postaci decyzji                                              **M**
> - selfcheck                                                               **M**
> - zaprogramowanie submodułu tyrana                                        **XXL**
> - zaprogramowanie submoduły konsylium                                     **XXL**

**e)** Zaprgoramowanie tymczasowych baz danych
> - unifikacja postaci danych                                               **M**
> - priorytetyzacja danych                                                  **L**
> - optymalizacja                                                           **M**
> - integrity selfcheck                                                     **M**

## **2.** Komponenty wewnętrzne modułu komunikacyjnego
**a)** Zaprogramowanie silnika szyfrowania
> - zaprojektowanie algorytmu szyfrującego i deszyfrującego                 **XXL**
> - zaprogramowanie dodatkowych zabezpieczeń komunikacji                    **L**
> - unifikacja postaci pakietów                                             **M**
> - selfcheck                                                               **M**

**b)** Zaprojektowanie postaci sieci
> - zaprojektowanie struktury dynamicznej siatki mesh                       **XL**
> - zaprojektowanie algorytmu autokonfiguracji połączeń                     **L**
> - implementacja mechanizmu redukcji tras                                  **L**
> - selfcheck                                                               **M**

**c)** Zaprogramowanie silnika komunikacyjnego
> - zaprojektowanie protokołu komunikacyjnego                               **L**
> - zaprogramowanie logiki diagnostycznej                                   **M**
> - zaprojektowanie logiki trybu tyran-pionek                               **L**
> - selfcheck                                                               **M**
> - datatraffic                                                             **M**

**d)** Zaprogramowanie menedżera danych sensorycznych
> - unifikacja postaci danych                                               **M**
> - logika sprawdzania poprawności danych                                   **L**
> - datatraffic                                                             **M**
> - selfcheck                                                               **M**

**e)** Zaprojektowanie menedżera diagnostycznego
> - integracja logiki diagnostycznej                                        **XL**
> - zaprojektowanie algorytmów diagnostycznych                              **L**
> - selfcheck                                                               **M**
> - datatraffic                                                             **M**

**f)** Dodanie niezbędnej logiki
> - logika obsługi kolizji pakietów                                         **L**
> - algorytm rozpoznawania opóźnień i ich kompensacji                       **M**
> - selfcheck                                                               **M**

## **3.** Komponenty wewnętrzne modułu diagnostycznego
**a)** Zaprojektowanie bezpośredniej komunikacji z modułem zabezpieczeń
> - unifikacja postaci komunikacji                                          **M**
> - zaprojektowanie tymczasowych baz danych                                 **L**
> - selfcheck                                                               **M**
> - datatraffic                                                             **M**
> - zaprojetkowanie logiki diagnostycznej                                   **XL**

**b)** Zaprojektowanie bezpośredniej komunikacji z modułem komunikacyjnym
> - unifikacja postaci komunikacji                                          **M**
> - zaprojektowanie tymczasowych baz danych                                 **L**
> - selfcheck                                                               **M**
> - datatraffic                                                             **M**
> - zaprojektowanie logiki diagnostycznej                                   **XL**

**c)** Zaprojektowanie systemu raportów
> - unifikacja postaci raportów                                             **M**
> - zaprojektowanie logiki generowania raportów                             **M**
> - selfcheck                                                               **M**
> - datatraffic                                                             **M**

**d)** Zaprojektowanie logiki diagnostycznej
> - zaprojektowanie algorytmów diagnostycznych dla węzłów sąsiednich        **XL**
> - zaprojektowanie wzorców zachowań                                        **L**
> - zaprojetkowanie testów integralnościowych                               **L**
> - zaprojetkowanie algorytmów diagnostycznych stanu własnego węzła         **XL**
> - selfcheck                                                               **M**
> - datatraffic                                                             **M**

**e)** Zaprojektowanie systemu autonaprawy sieci
> - zaprojektowanie algorytmów stabilizacji sieci po utracie węzłów         **XL**
> - zaprojektowanie monitoringu sieci                                       **XL**
> - zaprojetkowanie algorytmów wewnętrznych                                 **XL**

## **4.** Komponenty wewnętrze modułu zabezpieczeń
**a)** Zaprojektowanie komunikacji z innymi modułami
> - unifikacja postaci komunikacji                                          **M**
> - zaprojektowanie zabezpieczeń komunikacji                                **L**
> - zaprojektowanie algorytmów selfchecku komunikacji                       **M**

**b)** Zaprojektowanie selfchecka integralności modułów
> - zaprojektowanie algorytmów selfchecka integralności modułów             **L**
> - zaprojektowanie reakcji na wykrycie naruszeń                            **L**
> - zaprojektowanie systemu logowania i raportowania zdarzeń                **M**

**c)** Zaprojektowanie zabezpieczeń antywłamaniowych
> - synchronizacja detekcji anomalii                                        **M**
> - zaprojektowanie wspólnych logów bezpieczeństwa i diagnostyki            **L**

**d)** Zaprojektowanie systemu raportowego
> - unifikacja postaci raportowej                                          **M**
> - zaprogramowanie systemu generowania raportów                           **M**

**e)** Zaprojektowanie systemu autonaprawy węzła
> - zaprogramowanie algorytmów restartujących moduły                       **XL**
> - zaprojektowanie algorytmów restartu węzła                              **XL**
> - zaprogramowanie logiki autonaprawy                                     **XL**
