# 🛒 E-shop

## Changelog

### 🚩 23.9.2022

#### Zákaznický
- Možnost nastavit uživatelsky **měnu** a **zaokrouhlování** (bylo možné měnit pouze implementátorem)
- Zrychleno načítání kategorií
- Nová možnost tvorby individuálních filtrů na míru

#### Implementations
- BC-Break: Using `ShopConfig::$currency` and `ShopConfig::$precision` instead of `ConfigurationModel`
- New `ProductFilters` Service - Validating query filter parameters, unseting invalid values, handling product filter process
- Revised and rewritten `Categories` - Better optimization (1/2 query time)
