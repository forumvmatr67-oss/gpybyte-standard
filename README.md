# Gpybyte Independent Standard (GIS) – Version 1.0

**Registration number:** GIS-2025-001  
**Date of ratification:** 2025-05-12  
**Author:** Gosha 
**Domain:** https://gpybyte.dev  
**Repository:** https://github.com/forumvmatr67-oss/gpybyte-standard

## 1. Scope
This document defines three new units of digital information: **gpybyte**, **hpybyte**, and **ipybyte**, along with their symbols, relationships, and conversion rules.

## 2. Definitions

### 2.1 Base unit
The base unit is the **byte (B)**, as defined in ISO/IEC 80000-13.

### 2.2 The ipybyte
- **Name:** ipybyte
- **Symbol:** IpyB (uppercase) or ipyb (lowercase)
- **Value:** `1 ipybyte = 2⁹⁰ bytes = 1 237 940 039 285 380 274 899 124 224 B`

### 2.3 The hpybyte
- **Name:** hpybyte
- **Symbol:** HpyB / hpyb
- **Value:** `1 hpybyte = 1000 × ipybyte = 10³ × 2⁹⁰ B`

### 2.4 The gpybyte
- **Name:** gpybyte
- **Symbol:** GpyB / gpyb
- **Value:** `1 gpybyte = 1000 × hpybyte = 10⁶ × 2⁹⁰ B`

## 3. Relationship to other units
| Unit | Value in bytes | Value in ipybyte |
|------|----------------|------------------|
| 1 ipybyte | 2⁹⁰ B | 1 |
| 1 hpybyte | 10³ × 2⁹⁰ B | 1000 |
| 1 gpybyte | 10⁶ × 2⁹⁰ B | 1 000 000 |
| 1 yobibyte (YiB) | 2⁸⁰ B | 2⁻¹⁰ ipybyte ≈ 0.00097656 ipybyte |

## 4. Usage recommendations
- These units are intended for future large-scale data storage and transmission.
- Decimal prefixes (kilo-, mega-) should not be mixed with gpybyte/hpybyte/ipybyte to avoid confusion.

## 5. Copyright and license
This standard is released under the MIT License. You may freely use, copy, and modify it.

---
Signed: Gosha, 2025-05-12
