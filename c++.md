Ось зручна таблиця STL-контейнерів C++ у форматі:

> **Тип контейнера – Заголовочний файл – Базові методи**

| Тип контейнера           | Заголовочний файл | Базові методи                                                                                                                  |
| ------------------------ | ----------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| **`vector`**             | `<vector>`        | `size()`, `empty()`, `push_back()`, `pop_back()`, `at(i)`, `operator[]`, `front()`, `back()`, `clear()`, `insert()`, `erase()` |
| **`deque`**              | `<deque>`         | як `vector`, + `push_front()`, `pop_front()`                                                                                   |
| **`list`**               | `<list>`          | як `deque`, + `remove()`, `splice()`, `unique()`, `sort()`                                                                     |
| **`forward_list`**       | `<forward_list>`  | `push_front()`, `pop_front()`, `insert_after()`, `erase_after()`, `before_begin()`                                             |
| **`array`**              | `<array>`         | `size()`, `at()`, `front()`, `back()`, `fill()`, `data()`                                                                      |
| **`set`**                | `<set>`           | `insert()`, `erase()`, `find()`, `count()`, `size()`, `empty()`, `lower_bound()`, `upper_bound()`                              |
| **`map`**                | `<map>`           | `insert()`, `erase()`, `find()`, `count()`, `operator[]`, `at()`, `size()`, `empty()`                                          |
| **`multiset`**           | `<set>`           | як `set`, але дозволяє дублікати                                                                                               |
| **`multimap`**           | `<map>`           | як `map`, але дозволяє дублікати ключів                                                                                        |
| **`unordered_set`**      | `<unordered_set>` | як `set`, але швидший (хеш-таблиця), методи ті ж самі                                                                          |
| **`unordered_map`**      | `<unordered_map>` | як `map`, методи ті ж самі                                                                                                     |
| **`unordered_multiset`** | `<unordered_set>` | як `multiset`, але на основі хеш-таблиці                                                                                       |
| **`unordered_multimap`** | `<unordered_map>` | як `multimap`, але на основі хеш-таблиці                                                                                       |
| **`stack`**              | `<stack>`         | `push()`, `pop()`, `top()`, `size()`, `empty()`                                                                                |
| **`queue`**              | `<queue>`         | `push()`, `pop()`, `front()`, `back()`, `size()`, `empty()`                                                                    |
| **`priority_queue`**     | `<queue>`         | `push()`, `pop()`, `top()`, `size()`, `empty()`                                                                                |

---

