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