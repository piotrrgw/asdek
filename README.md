# Asystent Weryfikacji Wskazań ASDEK (DSAT Support Assistant)

Specjalistyczna aplikacja webowa wspierająca drużyny pociągowe oraz pracowników technicznych w szybkiej interpretacji wskazań urządzeń Detekcji Stanów Awaryjnych Taboru (DSAT/ASDEK). Narzędzie służy do precyzyjnej lokalizacji wskazanej osi i wagonu w składzie pociągu oraz sugeruje dalszy tok postępowania zgodnie z obowiązującymi przepisami.

## 📋 Podstawa regulaminowa

Logika działania aplikacji oraz procedury postępowania zostały opracowane w ścisłym oparciu o:
* **Instrukcję Ie-3 (PKP PLK)** – dotyczącą obsługi urządzeń do wykrywania zagrzanych łożysk osiowych i hamulców oraz płaskich miejsc na kołach.

## 🚀 Kluczowe funkcjonalności

### 1. Precyzyjna Lokalizacja (Axle & Wagon Finder)
System przelicza numer osi wskazany przez urządzenie ASDEK na konkretny wagon oraz umiejscowienie osi w tym wagonie (wózek, numer osi w wózku). Eliminuje to konieczność ręcznego przeliczania osi "na piechotę" w stresujących warunkach, redukując ryzyko pomyłki.

### 2. Wsparcie Decyzyjne (Procedury Ie-3)
Na podstawie wprowadzonych parametrów alarmu, aplikacja wyświetla odpowiedni algorytm postępowania (np. wymagane zatrzymanie, ograniczenie prędkości, sposób oględzin), pomagając użytkownikowi podjąć właściwe kroki zgodnie z instrukcją.

### 3. Obsługa Zróżnicowanego Taboru
Aplikacja posiada zaimplementowane algorytmy przeliczania osi dla różnych konfiguracji pociągów:

* **Składy klasyczne (Wagonowe):** Dowolna konfiguracja lokomotywy i wagonów.
* **Elektryczne Zespoły Trakcyjne (EZT):** Dedykowane moduły dla najpopularniejszych serii eksploatowanych w Polsce:
    * **ED74** (Pesa Bydgostia)
    * **ED160** (Stadler FLIRT)
    * **ED161** (Pesa DART)
    * **ED250** (Pendolino)

## 🤖 AI-Assisted Development

Projekt został zrealizowany w modelu **AI-Assisted** przy wsparciu generatywnej sztucznej inteligencji **Google Gemini**. Narzędzie to zostało wykorzystane do:
* Mapowania reguł logicznych z instrukcji Ie-3 na kod JavaScript.
* Opracowania struktur danych odwzorowujących układ osi w specyficznych pojazdach typu EZT (gdzie występują wózki Jakobs'a lub niestandardowe układy napędowe).
* Optymalizacji interfejsu (UX) pod kątem czytelności na urządzeniach mobilnych w warunkach terenowych.

## 🛠️ Technologie

* HTML5 / CSS3
* JavaScript (ES6+)
* RWD (Responsive Web Design) – aplikacja dostosowana do działania na smartfonach i tabletach służbowych.

## ⚠️ Nota Prawna (Disclaimer)

Aplikacja jest narzędziem pomocniczym (Wsparcie Decyzyjne). Mimo dołożenia wszelkich starań, aby algorytmy były zgodne z instrukcją Ie-3, wyłączną odpowiedzialność za bezpieczeństwo prowadzenia ruchu kolejowego, weryfikację stanu technicznego taboru oraz podjęte decyzje ponosi uprawniony pracownik kolei. W przypadku wątpliwości nadrzędne są zawsze zapisy w oficjalnych instrukcjach i regulaminach PKP PLK.
