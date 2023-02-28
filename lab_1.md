**Лабораторная работа №1**

**1. Скачайте библиотеку boost с помощью утилиты wget.**

wget https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz

**2. Разархивируйте скаченный файл в директорию ~/boost_1_69_0.**

tar -xvf boost_1_69_0.tar.gz

**3. Подсчитайте количество файлов в директории ~/boost_1_69_0 не включая вложенные директории.**

tree -L 1

<img width="413" alt="image" src="https://user-images.githubusercontent.com/126329578/221964277-4f9d6ffd-d145-4bc8-b5d9-ae126eb3d60a.png">

**_6 директорий и 12 файлов_**

**4. Подсчитайте количество файлов в директории ~/boost_1_69_0 включая вложенные директории.**

tree

**_5637 директорий и 61191 файлов_**

**5 Подсчитайте количество заголовочных файлов, файлов с расширением .cpp, сколько остальных файлов (не заголовочных и не .cpp).**

Для заголовочных файлов .h и .hpp, получим: find . -name "*.h" -o -name "*.hpp" | wc -l

<img width="356" alt="image" src="https://user-images.githubusercontent.com/126329578/221966675-13ee9dea-8a42-4073-aef3-405006c351c1.png">

**_15208_**

Для файлов с расширением .cpp получим: find . -name "*.cpp" | wc -l

<img width="361" alt="image" src="https://user-images.githubusercontent.com/126329578/221966635-e0650f81-0f7b-4793-a65e-8cda338ff206.png">

**_13774_**

Для остальных файлов получим: find . -not -name "*.h" -not -name "*.hpp" -not -name "*.cpp" | wc -l

<img width="421" alt="image" src="https://user-images.githubusercontent.com/126329578/221967049-9db5c634-b428-48df-a111-067f8f514cf4.png">

**_37859_**


