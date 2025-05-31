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
| **`stack`**              | `<stack>`         | `push()`, `pop()`, `top()`, `size()`, `empty()`                                                                                |
| **`queue`**              | `<queue>`         | `push()`, `pop()`, `front()`, `back()`, `size()`, `empty()`                                                                    |
| **`priority_queue`**     | `<queue>`         | `push()`, `pop()`, `top()`, `size()`, `empty()`                                                                                |

---

