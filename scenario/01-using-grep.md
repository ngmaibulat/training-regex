### Использование команды grep

-   Откроем `bash`
-   Перейдем в каталог `Desktop/github`
-   Посмотри содержимое каталога

### Задача 1 - Поиск слова в файле

```bash
echo "City:" > file.txt
echo "Ufa" >> file.txt
echo "Samara" >> file.txt
echo "Moscow" >> file.txt

cat file.txt

grep -F 'Ufa' file.txt
grep -F 'ufa' file.txt
```

Комментарий: Нашли слово `Ufa` в файле `file.txt`. Регистр важен

### Задача 2 - Поиск слова в файле без учета регистра

```bash
grep -i -F 'ufa' file.txt
```

Комментарий: регистр не важен

### Задача 3 - Поиск слова во всех файлах

```bash
grep -i -r 'ufa'
```

Комментарий: мы ищем слово `ufa` во всех файлах в текущем каталоге и подкаталогах.
Мы не указали имя файла для поиска

### Задача 4 - Поиск слова во всех файлах с выводом номера строки

```bash
grep -i -r -n 'ufa'
```

### Задача 6 - Подсветка найденного слова

```bash
grep -i --color 'ufa' file.txt
```

### Задача 7 - Вывод контекста в grep

Контекст - это несколько строк до и после найденной строки

```bash
grep -i --color -A 2 'ufa' file.txt
grep -i --color -B 2 'ufa' file.txt
grep -i --color -C 2 'ufa' file.txt
```
