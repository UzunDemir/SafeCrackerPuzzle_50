# 🧩 Safe Cracker 50: The "Broken Reality" Case

## 🇷🇺 README (Russian)

### Обзор

Репозиторий содержит исследование и решение деревянного пазла Safe Cracker 50. В процессе оцифровки и анализа было выявлено, что физический объект содержит критические производственные дефекты, делающие его решение невозможным без применения методов Data Science.

### Выявленные аномалии

* **Зеркальный саботаж:** 4 из 5 дисков были напечатаны в зеркальном отражении относительно математической модели.
* **Арифметический баг:** В секторе №14 обнаружена аппаратная ошибка — сумма чисел в любом положении на 10 единиц меньше целевой (40 вместо 50).

### Реализация

* Поиск решения через перебор всех  комбинаций.
* Алгоритм автоматического обнаружения системных сдвигов и опечаток.
* Применение `np.flip()` для коррекции зеркальности дисков.
* Финальный патч данных, восстанавливающий логическую целостность пазла.

---

## 🇺🇸 README (English)

### Overview

This repository features the reverse engineering and solving of the Safe Cracker 50 wooden puzzle. During the data analysis phase, it was mathematically proven that the physical unit contains critical manufacturing defects, rendering it unsolvable by traditional means.

### Discovered Anomalies

* **Mirror Sabotage:** 4 out of 5 disks were engraved in reverse (mirrored) order.
* **Arithmetic Bug:** Sector #14 was identified as having a "hardware" error — its total is hardcoded to be 10 units short (40 instead of 50).

### Implementation

* Brute-force solver covering all  possible rotations.
* Anomaly detection algorithm to identify systemic offsets and typos.
* `np.flip()` implementation to counter-mirror the data arrays.
* Digital data patching to achieve a perfect 16/16 sector match.

---

## 📊 Results

| Feature | Raw Physical State | Patched Digital State |
| --- | --- | --- |
| **Disk Orientation** | Mirrored (4/5) | Corrected ✅ |
| **Target Sum** | 50 | 50 |
| **Sector 14 Sum** | 40 | 50 ✅ |
| **Success Rate** | 0% | 100% ✅ |

### Tech Stack

`Python`, `NumPy`, `Matplotlib`

---
