Introduction
=
Библиотека string.h является основной библиотекой языка С по обработке строк. В рамках этого проекта я релизовала функцию sscanf, которая считывает данные и записывает их в переменные.

 ```int sscanf(const char *str, const char *format, ...)``` - считывает форматированный ввод из строки.
 
где:
- **str** − Это С-строка, которую функция обрабатывает в качестве источника для извлечения данных;
- **format** −  это С-строка, содержащая один или несколько следующих элементов: пробельный символ, непробельный символ и спецификаторы формата. Спецификатор формата для сканирующих функций следует прототипу:

  **% [*] [ширина] [длина] спецификатор**.

## Cпецификаторы

  | № | Спецификатор | Результат sscanf |
  
| 1 | c | Символ |

| 2 | d | Знаковое десятичное целое число |

| 3 | i | Знаковое целое число (может быть десятичным, восьмеричным или шестнадцатеричным) |

| 4 | e | Десятичное число с плавающей точкой или научная нотация (мантисса/экспонента) |

| 5 | E | Десятичное число с плавающей точкой или научная нотация (мантисса/экспонента) |

| 6 | f | Десятичное число с плавающей точкой или научная нотация (мантисса/экспонента) |

| 7 | g | Десятичное число с плавающей точкой или научная нотация (мантисса/экспонента) |

| 8 | G | Десятичное число с плавающей точкой или научная нотация (мантисса/экспонента) |

| 9 | o | Беззнаковое восьмеричное число |

| 10 | s | Строка символов |

| 11 | u | Беззнаковое десятичное целое число |

| 12 | x | Беззнаковое шестнадцатеричное целое число (любые буквы) |

| 13 | X | Беззнаковое шестнадцатеричное целое число (любые буквы) |

| 14 | p | Адрес указателя |

| 15 | n | Количество символов, считанных до появления %n |

| 16 | % | Символ % |

## Ширина

| № | Ширина | Описание |

| 1	| (число) | Максимальное количество читаемых символов.|

## Длина

| № | Длина | Описание |

| 1 | h | Аргумент интерпретируется как короткое int или короткое int без знака (применяется только к целочисленным спецификаторам: i, d, o, u, x и X). |

| 2 | l | Аргумент интерпретируется как длинное int или длинное int без знака для целочисленных спецификаторов (i, d, o, u, x и X) и как широкий символ или строка широких символов для спецификаторов c и s. |

| 3 | L | Аргумент интерпретируется как длинный double (применяется только к спецификаторам с плавающей точкой − e, E, f, g и G). |

## Флаг [*]

| * | Если после ' % ' следует ' * ', то результат считывается, но не присваивается переменной. | 

## Description

- В папке src реализация функции sscanf под названием `s21_sscanf`. 

- В mainscan.c один простой пример работы функции, вы можете попробовать свои примеры самостоятельно.

- Если не работали с cmake: Для запуска перейти в папку build, выполнить команды в терминале:

      cmake ..
      make


 затем запустить испольняемый файл с помощью команды:

     ./sscanf
 



