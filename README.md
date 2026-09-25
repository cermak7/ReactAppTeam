# CRM - Refaktoring a převzetí projektu (Týmový projekt)

Tento repozitář obsahuje kód pro výběrové řízení na nového vývojového partnera pro existující CRM software. Cílem projektu je převzít stávající React aplikaci, refaktorovat vybrané části, opravit chyby a převést sestavování projektu z Webpacku na Vite.

**Původní repozitář (zdroj):** [https://github.com/lmasic/crmWAcv](https://github.com/lmasic/crmWAcv)

## 👥 Tým a rozdělení rolí

| Člen týmu | Role | Zodpovědnost / Úkol |
| :--- | :--- | :--- |
| **Čermák** | **GIT Master / Vývojář** | Koordinace projektu, příprava repozitáře, code review, odevzdání konečné verze. Komunikace s vyučujícími. Převod na **Vite**. + **Úkol 5** |
| **Buzek** | Vývojář | **Úkol 1:** Implementace React Routing |
| **Karabáček** | Vývojář | **Úkol 2:** Oprava chyby překreslování tabulky v sekci Zasílání |
| **Hron** | Vývojář | **Úkol 3:** Vytvoření univerzální tabulkové komponenty |
| **Berger** | Vývojář | **Úkol 4:** Identifikace a úklid nepoužívaných souborů/komponent |

## 📋 Rozpis úkolů (Zadání)

1. **React Routing (Buzek)**
   * Předělat zobrazení kontaktů, schůzek a akcí pomocí React Routeru.
   * Cíl: Zrušit stávající plovoucí vrstvy (modals) a nahradit je plnohodnotnými URL routami.
2. **Oprava bugu - Zasílání (Karabáček)**
   * V sekci zasílání je chyba: Při druhém uložení stavu se nepřekreslí tabulka, ačkoliv se data na pozadí správně uloží.
   * Cíl: Zjistit příčinu chybějícího re-renderu a opravit ji.
3. **Univerzální komponenta Tabulka (Hron)**
   * Zobrazení dat v tabulkách se v aplikaci často opakuje.
   * Cíl: Vytvořit znovupoužitelnou React komponentu (inspirovanou funkčností v sekci "Firmy") a naimplementovat ji napříč kódem.
4. **Úklid kódu (Berger)**
   * Cíl: Identifikovat a bezpečně odstranit nepoužívané komponenty a soubory, které v projektu zbyly po předchozí firmě.
5. **Refaktoring backendu / API (Čermák)**
   * Soubor `requests.php` je děsivě veliký a nepřehledný.
   * Cíl: Rozdělit tento soubor na menší logické celky a zpřehlednit strukturu API volání.

## ⚙️ Technické informace a lokální spuštění

Projekt byl původně postaven na Webpacku. Nyní je (nebo v rámci přípravy bude) zmigrován na **Vite** pro rychlejší vývoj.

**Přístupové údaje do testovacího prostředí:**
* **Login:** `reader`
* **Heslo:** `1234OLe`

### Jak spustit projekt

1. Naklonujte si repozitář:
   ```bash
   git clone [URL_Vaseho_Noveho_Repozitare]
   cd [nazev_slozky]
