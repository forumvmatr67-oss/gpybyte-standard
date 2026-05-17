# jpybyte – спецификация единицы (GIS v2.0)

**Статус:** СТАБИЛЬНЫЙ  
**Версия стандарта:** GIS 2.0  
**Дата:** 2025-05-17  
**Автор:** Gosha  
**Лицензия:** Apache 2.0 (см. `LICENSE` в корне репозитория)

---

## 1. Определение

**jpybyte** (символы: `JpyB` или `jpyb`) – четвёртая единица в иерархии **Gpybyte Independent Standard (GIS)**.
1 jpybyte = 1000 × gpybyte
1 jpybyte = 1 000 000 × hpybyte
1 jpybyte = 1 000 000 000 × ipybyte
1 jpybyte = 10⁹ × 2⁹⁰ байт

### 1.1 Точное значение в байтах
1 jpybyte = 1 237 940 039 285 380 274 899 124 224 000 000 000 байт

text

Это число содержит 36 десятичных цифр.

---

## 2. Место в системе GIS

Гибридная (двоично-десятичная) шкала:
ipybyte (2⁹⁰ B)
↓ ×1000
hpybyte (10³ × ipybyte)
↓ ×1000
gpybyte (10⁶ × ipybyte)
↓ ×1000
jpybyte (10⁹ × ipybyte) ← текущая единица
↓ ×1000 (следующие)
kpybyte, lpybyte, mpybyte, …

text

---

## 3. Отношение к другим единицам

| Единица | Значение в jpybyte |
|---------|--------------------|
| 1 ipybyte | 0,000 000 001 (10⁻⁹) |
| 1 hpybyte | 0,000 001 (10⁻⁶) |
| 1 gpybyte | 0,001 (10⁻³) |
| 1 jpybyte | 1 |
| 1 kpybyte | 1 000 (10³) |

### Сравнение с йобибайтом (YiB)

- 1 YiB ≈ 0,000 000 000 97656 jpybyte  
- 1 jpybyte ≈ 1 099 511 627 776 YiB

---

## 4. Код для разработчиков

### Python

```python
# GIS units – версия 2.0
IPY = 2 ** 90
HPY = 1000 * IPY
GPY = 1000 * HPY
JPY = 1000 * GPY   # jpybyte

def to_bytes(value, unit):
    return value * unit

print(f"1 jpybyte = {to_bytes(1, JPY)} bytes")
