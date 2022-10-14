# 🛒 E-shop

## Changelog

### 🚩 14.10.2022
- Možnost povolit **Způsoby dopravy** zvlášť pro každého zákazníka *(podobně jako **Způsoby platby**)*
- Zákazníci mohou nově zažádat o obnovu hesla 1x za hodinu

### 🚩 12.10.2022

#### Zákaznický
- Možnost nastavovat **Způsobům dopravy** minimální váhu
- Možnost nahrávat vlastní obrázky ke **Způsobům dopravy**
- Možnost nahrávat vlastní obrázky ke **Způsobům platby**
- Možnost povolit **Způsob dopravy** od zadané minimální váhy objednávky *(vhodné např. pro paletovou dopravu)*

### 🚩 27.9.2022

#### Zákaznický
- Možnost nastavovat produktům **jakost**
- Možnost filtrovat dle **jakosti** produktu (jak v administraci, tak na e-shopu)
- Přidán nový sloupeček **jakost** do tabulky produktů (skrytý ve výchozím stavu)
- Seznam povolených jakostí a výchozí jakost je možné nastavit v `Konfigurace -> Obchod`
- Seznam všech jakostí je možné na žádost upravit pro každý projekt zvlášť

### 🚩 23.9.2022

#### Zákaznický
- Možnost nastavit uživatelsky **měnu** a **zaokrouhlování** (bylo možné měnit pouze implementátorem)
- Zrychleno načítání kategorií
- Nová možnost tvorby individuálních filtrů na míru
- Nová možnost upravovat zákaznické informace z administrace (kontaktní, fakturační i dodací údaje)
- Nová možnost ověřovat zákaznický e-mail
- Nová možnost přihlásit se do zákaznického účtu
- Nová možnost omezovat přístup do zákaznických účtů dle role uživatelského účtu
- Nová možnost povolit / zakázat uživateli jednotlivé funkce zákaznického účtu - přehled, úprava, aktivace a přihlašování
- Opravena chyba při ořezávání obrázků **Prodejců**

#### Implementations
- BC-Break: Using `ShopConfig::$currency` and `ShopConfig::$precision` instead of `ConfigurationModel`
- New `ProductFilters` Interface - Validating query filter parameters, unseting invalid values, handling product filter process
- Revised and rewritten `Categories` - Better optimization (1/2 query time)

### 🚩 20.9.2022

#### Zákaznický
- Nový panel **Statistiky**:
  - Informace o tržbách, dokočených objednávkách a nových zákaznících
  - Možnost zvolit období - Den, Týden, Měsíc, Rok (posledních 365 dní) a Aktuální rok (data od začátku roku do aktuálního dne)
  - Možnost porovnávat data s minulým obdobím (v případě volby **Aktuální rok** poté od začátku minulého roku do aktuálního data minulého roku)
- Nová možnost označit **Stav objednávky** jako **Konečný stav**
  - **Konečný stav** objednávky určuje úspěšné dokončení objednávky
  - Veškeré objednávky v **konečném stavu** se poté započítávají do statistik
 - Přepracováno grafické rozhraní **Nastavení obchodu**
