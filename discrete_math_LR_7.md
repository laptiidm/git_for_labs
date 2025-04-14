Добре! Побудуємо **ДДНФ (диз'юнктивну нормальну форму)** та **ДКНФ (кон'юнктивну нормальну форму)** для логічної функції:

\[
f(x, y, z, t) = (xy \vee x\overline{y}) \vee ((\overline{x} \vee y)(z \vee \overline{t})(\overline{x} \vee \overline{y})(t \vee z))
\]

---

### 🔹 Крок 1: Побудуємо таблицю істинності

Для 4 змінних (x, y, z, t) буде 16 комбінацій. Знайдемо значення функції для кожної.

| x | y | z | t | f(x,y,z,t) |
|---|---|---|---|-------------|
| 0 | 0 | 0 | 0 | 1 |
| 0 | 0 | 0 | 1 | 1 |
| 0 | 0 | 1 | 0 | 1 |
| 0 | 0 | 1 | 1 | 1 |
| 0 | 1 | 0 | 0 | 0 |
| 0 | 1 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 1 |
| 0 | 1 | 1 | 1 | 0 |
| 1 | 0 | 0 | 0 | 1 |
| 1 | 0 | 0 | 1 | 1 |
| 1 | 0 | 1 | 0 | 1 |
| 1 | 0 | 1 | 1 | 1 |
| 1 | 1 | 0 | 0 | 0 |
| 1 | 1 | 0 | 1 | 0 |
| 1 | 1 | 1 | 0 | 1 |
| 1 | 1 | 1 | 1 | 0 |

---

### 🔹 Крок 2: ДДНФ (Диз'юнктивна ДНФ)

ДДНФ — це диз'юнкція всіх **мінтермів**, для яких функція дорівнює 1.

Мінтерм — це кон'юнкція змінних або їх заперечень, яка дорівнює 1 **лише для одного набору значень**.

Функція дорівнює 1 для наборів:
- 0000 → \( \overline{x}\,\overline{y}\,\overline{z}\,\overline{t} \)
- 0001 → \( \overline{x}\,\overline{y}\,\overline{z}\,t \)
- 0010 → \( \overline{x}\,\overline{y}\,z\,\overline{t} \)
- 0011 → \( \overline{x}\,\overline{y}\,z\,t \)
- 0110 → \( \overline{x}\,y\,z\,\overline{t} \)
- 1000 → \( x\,\overline{y}\,\overline{z}\,\overline{t} \)
- 1001 → \( x\,\overline{y}\,\overline{z}\,t \)
- 1010 → \( x\,\overline{y}\,z\,\overline{t} \)
- 1011 → \( x\,\overline{y}\,z\,t \)
- 1110 → \( x\,y\,z\,\overline{t} \)

**Отже, ДДНФ:**

\[
f(x,y,z,t) = (\overline{x}\,\overline{y}\,\overline{z}\,\overline{t}) \vee (\overline{x}\,\overline{y}\,\overline{z}\,t) \vee (\overline{x}\,\overline{y}\,z\,\overline{t}) \vee (\overline{x}\,\overline{y}\,z\,t) \vee (\overline{x}\,y\,z\,\overline{t}) \vee (x\,\overline{y}\,\overline{z}\,\overline{t}) \vee (x\,\overline{y}\,\overline{z}\,t) \vee (x\,\overline{y}\,z\,\overline{t}) \vee (x\,\overline{y}\,z\,t) \vee (x\,y\,z\,\overline{t})
\]

---

### 🔹 Крок 3: ДКНФ (Кон'юнктивна КНФ)

ДКНФ — це кон'юнкція всіх **макстермів**, де функція дорівнює 0.

Макстерм — диз'юнкція змінних або їх заперечень, яка дорівнює 0 **лише для одного набору значень**.

Набори, де \( f = 0 \):
- 0100 → \( \overline{x} \vee \overline{y} \vee \overline{z} \vee \overline{t} \)
- 0101 → \( \overline{x} \vee \overline{y} \vee \overline{z} \vee t \)
- 0111 → \( \overline{x} \vee \overline{y} \vee z \vee t \)
- 1100 → \( \overline{x} \vee y \vee \overline{z} \vee \overline{t} \)
- 1101 → \( \overline{x} \vee y \vee \overline{z} \vee t \)
- 1111 → \( \overline{x} \vee y \vee z \vee t \)

**Отже, ДКНФ:**

\[
f(x,y,z,t) = (\overline{x} \vee \overline{y} \vee \overline{z} \vee \overline{t}) \wedge (\overline{x} \vee \overline{y} \vee \overline{z} \vee t) \wedge (\overline{x} \vee \overline{y} \vee z \vee t) \wedge (\overline{x} \vee y \vee \overline{z} \vee \overline{t}) \wedge (\overline{x} \vee y \vee \overline{z} \vee t) \wedge (\overline{x} \vee y \vee z \vee t)
\]

---

Якщо хочеш, я можу:
- Перевести це у вигляд булевих виразів у коді;
- Побудувати логічну схему;
- Спробувати спростити ДДНФ або ДКНФ.

Що далі? 😊