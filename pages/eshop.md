# 🛒 E-shop

## Changelog

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
