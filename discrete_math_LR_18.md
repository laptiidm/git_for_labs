
---

## **Лабораторна робота: Знаходження найкоротшого шляху за алгоритмом Дейкстри**
### Дмитро Лаптій. Варіант 5

### **Мета роботи:**

Навчитися застосовувати алгоритм Дейкстри для пошуку найкоротшого шляху у зваженому графі.

---

### **Вхідні дані:**

Граф задано у вигляді прямокутної сітки (матриці вузлів 5×6). Вузли з'єднані горизонтальними та вертикальними ребрами з відповідними вагами.

#### Горизонтальні ребра (між вузлами одного рядка):

```python
horizontal = [
  [8, 4, 6, 2, 4],    # Рядок 0
  [2, 1, 1, 1, 5],    # Рядок 1
  [1, 1, 3, 6, 1],    # Рядок 2
  [3, 7, 5, 8, 5],    # Рядок 3
  [3, 3, 4, 7, 7]     # Рядок 4
]
```

#### Вертикальні ребра (між вузлами сусідніх рядків):

```python
vertical = [
  [4, 1, 4, 7, 7, 5],   # Між рядками 0 та 1
  [3, 1, 3, 7, 7, 2],   # Між рядками 1 та 2
  [2, 7, 3, 1, 3, 8],   # Між рядками 2 та 3
  [4, 3, 2, 7, 3, 1]    # Між рядками 3 та 4
]
```

---

### **Постановка задачі:**

Знайти найкоротший шлях між вершинами **V₀ = (0, 0)** і **V* = (4, 5)*\* з урахуванням ваг усіх горизонтальних і вертикальних ребер.

---

### **Алгоритм Дейкстри (опис кроків):**

1. Ініціалізуємо всі відстані як нескінченність, крім початкової вершини — їй присвоюємо 0.
2. Створюємо множину неперевірених вершин.
3. Знаходимо вершину з найменшою відстанню, обходимо всіх її сусідів і оновлюємо для них відстані, якщо шлях через поточну вершину коротший.
4. Повторюємо, поки не обробимо всі вершини або не знайдемо цільову вершину.
5. Відновлюємо найкоротший шлях з кінцевої вершини до початкової, рухаючись назад через збережені попередні вузли.

---

### **Результати обчислень:**

#### ✅ Найкоротший шлях:

```
(0, 0) → (1, 0) → (1, 1) → (1, 2) → (1, 3) → (1, 4) → (1, 5) → (2, 5) → (3, 5) → (4, 5)
```

#### 🧮 Загальна вага шляху: **25**

---

### **Висновок:**

У результаті застосування алгоритму Дейкстри було знайдено найкоротший шлях у зваженому графі розміром 5×6. Отриманий шлях дозволяє з найменшими витратами (вага = 25) дістатися з вершини (0, 0) до вершини (4, 5).

---

