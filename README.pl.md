# Menadżer Spolszczeń

Menadżer Spolszczeń to aplikacja [Bazy Spolszczeń](https://bazaspolszczen.pl), katalogu polskich spolszczeń gier
tworzonych przez fanów. Znajduje zainstalowane gry, instaluje do nich spolszczenia z Bazy Spolszczeń i dba o ich
aktualność. Każdą zmianę wprowadzoną w grze da się cofnąć.

*In English: [README.md](README.md).*

To repozytorium służy tylko do publikowania wydań aplikacji. Jej kod źródłowy jest w repozytorium
[JustModIt Manager](https://github.com/GrzybDev/JustModIt-Manager).

## Pobieranie

Instalator `MenadzerSpolszczen-win-Setup.exe` jest w [najnowszym
wydaniu](https://github.com/GrzybDev/MenadzerSpolszczen/releases/latest). Aplikacja instaluje się dla bieżącego
użytkownika Windows, bez uprawnień administratora, a potem sama się aktualizuje.

- Wymaga Windows 10 lub 11 w wersji 64-bitowej.
- Wydania oznaczone jako „Pre-release” to wczesne wersje, w których mogą się zdarzać niedociągnięcia.
- Aplikacja i jej instalator są podpisane cyfrowo przez „Open Source Developer, Marek Grzyb”.

## Co potrafi

- **Znajduje gry** ze Steama, GOG-a (GOG Galaxy, instalatory offline i Heroic) i Epic Games Store (Epic Games Launcher,
  Heroic i Legendary) i na bieżąco śledzi zmiany w sklepach, bez przeszukiwania dysków.
- **„Moje gry”** pokazują gry, do których Baza Spolszczeń ma ukończone spolszczenie pasujące do zainstalowanej wersji
  gry, a **„Katalog”** pozwala przejrzeć wszystkie spolszczenia ze strony.
- **Instaluje spolszczenia** jednym kliknięciem albo automatycznie, najpierw sprawdza, czy spolszczenie pasuje do
  zainstalowanej wersji gry, i nigdy nie rusza gry, która jest uruchomiona albo właśnie aktualizowana przez sklep.
- **Pozwala wybrać spolszczenie**, gdy tę samą grę przetłumaczyło kilka grup; o instalacjach automatycznych decydują
  grupy wskazane w ustawieniach jako preferowane.
- **Dba o aktualność**: instaluje nowe wydania zainstalowanych spolszczeń i przywraca spolszczenie, gdy aktualizacja gry
  je nadpisze. Do gry, która oficjalnie ma język polski, spolszczenie nigdy nie jest instalowane automatycznie.
- **Pozwala cofnąć wszystko**, także bez internetu: zachowuje oryginalne pliki (domyślnie w ukrytym folderze
  `.menadzer-spolszczen` w folderze gry), a instalację przerwaną przez awarię lub brak prądu sama wycofuje.
- **Działa po cichu** w zasobniku systemowym i uruchamia się razem z Windows; tę opcję można wyłączyć.
- **Kreator spolszczeń**, dostępny dla tłumaczy w trybie twórcy, buduje paczki ze spolszczeniem z folderu z
  przetłumaczonymi plikami.

## Prywatność

Aplikacja nie zbiera danych o sposobie korzystania z niej. Łączy się tylko z Bazą Spolszczeń (lista spolszczeń, paczki
i obrazy), z GitHubem (aktualizacje aplikacji) i z serwerami obrazów pokazywanych przez stronę. Pobranie paczki liczy
się na stronie spolszczenia tak samo jak pobranie ze strony.

## Odinstalowywanie

Aplikację odinstalowuje się w Ustawieniach Windows, w sekcji Aplikacje. Zainstalowane spolszczenia zostają w grach:
aby odzyskać oryginalne pliki, najpierw trzeba odinstalować spolszczenia w aplikacji. Ustawienia i zapisy aplikacji
zostają w `%LOCALAPPDATA%\BazaSpolszczen\MenadzerSpolszczen`, więc po ponownej instalacji wszystko wraca na swoje
miejsce.

## Licencja

Kod aplikacji jest wolnym oprogramowaniem na licencji GNU General Public License w wersji 3 lub późniejszej. Nazwy i
logotypy Bazy Spolszczeń i Menadżera Spolszczeń nie są objęte tą licencją. Szczegóły, a także informację, gdzie znaleźć
kod źródłowy każdego wydania, zawiera [LICENSE.md](LICENSE.md).
