Написать программу, выводящую текст песни "99 бутылок пива". Общий вид куплета:

    [n] бутылок пива на стене, [n] бутылок пива!
    Возьми одну, передай мне, [n-1] бутылок пива на стене.

Куплеты должны быть разделены пустой строкой.

Текст куплета должен соответствтовать нормам русского языка:

    1 бутылка
    22 бутылки
    50 бутылок
    ...

Последние два куплета должны выглядеть так:

    Последняя бутылка пива на стене, последняя бутылка пива!
    Возьми её, передай мне, нет бутылок пива на стене.

    Нет бутылок пива на стене, нет бутылок пива!
    Сходи в магазин, купи ещё, 99 бутылок пива на стене.

Программа должна предоставлять собой один .py модуль (файл), предоставляющий внешний API в виде двух функций.
Первая функция выводит полный текст песни:

    def song() -> str:
        ...

Вторая функция выводит текст песни частично, начиная и заканчивая куплетами, заданными двумя целыми числами:

    def verses(upper, lower) -> str:
        ...

Пример:

    >>> verses(99, 98)
    99 бутылок пива на стене, 99 бутылок пива!
    Возьми одну, передай мне, 98 бутылок пива на стене.

    98 бутылок пива на стене, 98 бутылок пива!
    Возьми одну, передай мне, 97 бутылок пива на стене.

Полный текст песни для тестов: song.txt
