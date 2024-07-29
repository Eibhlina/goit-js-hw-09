# Zadanie 1. Galeria obrazów

Wykonaj to zadanie w plikach 01-gallery.html i 01-gallery.js.

W poprzednim zadaniu domowym utworzyłeś/aś galerię obrazów przy użyciu delegowania zdarzeń i dodałeś/aś okno modalne za pośrednictwem biblioteki CDN, aby wyświetlać pełnowymiarową wersję obrazu.

Tworzenie galerii jest codziennym zadaniem dla programistów, ale ręczne pisanie ich za każdym razem jest zbyt czasochłonne. W tym celu istnieją biblioteki, które implementują całą logikę galerii.

Utwórz tę samą galerię, ale przy użyciu biblioteki SimpleLightbox, która zajmie się kliknięciami obrazów, otwieraniem i zamykaniem okna modalnego oraz przewijaniem obrazów za pomocą klawiatury.


Zwróć uwagę na następujące niuanse:

* Nie trzeba już wdrażać delegowania zdarzeń, biblioteka SimpleLightbox sama będzie śledzić kliknięcia na kartach galerii.
* Nie potrzebujesz już biblioteki do tworzenia okna modalnego, ta funkcjonalność jest wbudowana w bibliotece SimpleLightbox.

Wykonaj to zadanie w plikach gallery.html i gallery.js. Podziel to zadanie na kilka podzadań.



Użyj kodu z poprzedniego zadania domowego i dokonaj jego refaktoryzacji. Nie musisz pisać wszystkiego od nowa. Na przykład, tworzenie elementów galerii pozostanie bez zmian. Ale kod delegujący i otwierający okno modalne powinien zostać usunięty.

Dodaj bibliotekę SimpleLightbox jako zależność projektu za pomocą npm . Aby dołączyć kod CSS biblioteki do projektu, należy dodać kolejny import, oprócz tego opisanego w dokumentacji.

Następnym krokiem jest inicjalizacja biblioteki po utworzeniu i dodaniu elementów galerii do ul.gallery. Aby to zrobić, przeczytaj dokumentację SimpleLightbox, zwłaszcza sekcje „Usage” i „Markup”.

Następnie zapoznaj się z dokumentacją w sekcji „Opcje” i dodaj wyświetlane podpisy do obrazów z atrybutu alt. Niech podpis będzie na dole i pojawi się 250 milisekund po otwarciu okna modalnego.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Zadanie 2. Formularz zwrotny

Wykonaj to zadanie w plikach 02-form.html i 02-form.js.

Dodaj do HTML znaczniki formularza. W JS napisz skrypt, który będzie zapisywał wartości pól w pamięci lokalnej, gdy użytkownik coś wpisze.


Wykonaj to zadanie w plikach feedback.html i feedback.js.

Podziel go na kilka podzadań:

1. Korzystając z delegowania, śledź zdarzenie input w formularzu i za każdym razem zapisuj obiekt z polami email i message do pamięci lokalnej, w której przechowywane są bieżące wartości pól formularza. Niech kluczem dla magazynu będzie ciąg „feedback-form-state”.
2. Po załadowaniu strony sprawdź stan pamięci, a jeśli są tam przechowywane dane, wypełnij nimi pola formularza. W przeciwnym razie pola powinny być puste.
3. Podczas submitu formularza wyczyść pamięć formularza i pola, a następnie wyświetl w konsoli obiekt z polami e-mail, message i ich aktualnymi wartościami.






