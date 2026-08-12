# Wydania — Optima Integrator i OptimaSync

Instalatory dwóch produktów do Comarch ERP Optima:

- **Optima Integrator** (`OptimaIntegrator-setup-*.exe`) — REST API + serwer MCP dla
  Claude Desktop. Katalog główny tego repozytorium.
- **OptimaSync** (`sync/OptimaSync-setup-*.exe`) — synchronizacja ze sklepami
  (WooCommerce, PrestaShop, Allegro): zamówienia, stany, ceny, kartoteki.

Oba wymagają pliku licencji `licencja.lic` wystawianego indywidualnie — bez niego
program się uruchomi, ale odmówi pracy i napisze dlaczego. W sprawie licencji
(również **wersji próbnej**) skontaktuj się z dostawcą.

**Wymagania:** Windows 10/11 64-bit oraz Comarch ERP Optima **2026.5 lub nowsza**,
zainstalowana lokalnie na tym samym komputerze. Od 2026.5 Optima jest 64-bitowa;
dla starszej, 32-bitowej Optimy ostatnie pasujące wydania to Integrator **1.3.0**
i OptimaSync **1.0.54** — instalator nowszej wersji odmówi instalacji, zamiast
zepsuć działającą konfigurację.

**Instalacja:** pobierz najnowszy instalator, uruchom, a po instalacji umieść
`licencja.lic` w folderze programu (domyślnie `C:\OptimaIntegrator` lub `C:\OptimaSync`).

**Aktualizacja:** w oknie programu przycisk „Zainstaluj aktualizację" robi wszystko
sam — pobiera, sprawdza sumę kontrolną i instaluje. Konfiguracja, licencja i dane
zostają zachowane. Instalator uruchomiony ręcznie działa tak samo.

`version.json` (oraz `sync/version.json`) opisują dostępne wydania wraz z zakresem
wersji Optimy — program sam wybiera to, które pasuje do zainstalowanej u Ciebie Optimy.
