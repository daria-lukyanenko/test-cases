Практическая задача 1.3.4 Проверяемое задание «Функциональное тестирование»

Блок 1: Позитивные сценарии: валидные email-адреса

Название: "Ввод валидного email-адреса"

Шаги воспроизведения:

1. Ввести адрес "a1b2c3@academy.ru" в поле для email.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: появляется alert с текстом "Прекрасный email-адрес".

///

Название: "Ввод email-адреса с поддоменами"

Шаги воспроизведения:

1. Ввести адрес "user.name@sub.domain.co.uk" в поле для email.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: появляется alert с текстом "Прекрасный email-адрес".

///

Название: "Ввод email-адреса с цифрами в локальной части"

Шаги воспроизведения:

1. Ввести адрес "lalala123@mail.com" в поле для email.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: появляется alert с текстом "Прекрасный email-адрес".

///

Название: "Ввод email-адреса с допустимыми спецсимволами в локальной части"

Шаги воспроизведения:

1. Ввести адрес "meow!meow#$%&'\*+-/=?^\_`{|}~@example.com" в поле для email.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: появляется alert с текстом "Прекрасный email-адрес".

///

Название: "Ввод email-адреса с точкой в локальной части"

Шаги воспроизведения:

1. Ввести адрес "firstname.lastname@domain.com" в поле для email.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: появляется alert с текстом "Прекрасный email-адрес".

Блок 2: Негативные сценарии: невалидные email-адреса

Название: "Ввод email-адреса без символа "@" "

Шаги воспроизведения:

1. Ввести адрес "user156!+example.com" в поле для email.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: над кнопкой "Проверить" появляется текст ошибки красного цвета "Введен некорректный email".

///

Название: "Ввод email-адреса без доменной части"

Шаги воспроизведения:

1. Ввести адрес "usermeow279@" в поле для email.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: над кнопкой "Проверить" появляется текст ошибки красного цвета "Введен некорректный email".

///

Название: "Ввод email-адреса без локальной части"
Шаги воспроизведения:

1. Ввести адрес "@example.com" в поле для email.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: над кнопкой "Проверить" появляется текст ошибки красного цвета "Введен некорректный email".

///

Название: "Ввод email-адреса с пробелом в локальной части"

Шаги воспроизведения:

1. Ввести адрес "usermeow123 67!name@example.com" в поле для email.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: над кнопкой "Проверить" появляется текст ошибки красного цвета "Введен некорректный email".

///

Название: "Ввод email-адреса с недопустимым символом "()" "

Шаги воспроизведения:

1. Ввести адрес "name()@example.com" в поле для email.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: над кнопкой "Проверить" появляется текст ошибки красного цвета "Введен некорректный email".

///

Название: "Ввод email-адреса с точкой в начале локальной части "

Шаги воспроизведения:

1. Ввести адрес ".username@example.com" в поле для email.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: над кнопкой "Проверить" появляется текст ошибки красного цвета "Введен некорректный email".

///

Название: "Ввод email-адреса с точкой в конце доменной части"

Шаги воспроизведения:

1. Ввести адрес "firstrname!@example.com." в поле для email.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: над кнопкой "Проверить" появляется текст ошибки красного цвета "Введен некорректный email".

Блок 3: Граничные значения и пустые значения

Название: "Отправка пустой строки"

Шаги воспроизведения:

1. Оставить поле для email пустым.
2. Нажать кнопку "Проверить".
   Ожидаемый результат: над кнопкой "Проверить" появляется текст ошибки красного цвета "Введен некорректный email".

///

Название: "Ввод длинных, но допустимых строк"

Шаги воспроизведения:

1. Ввести длинный, но корректный email ( "t".repeat(64) + "@" + "u".repeat(185) + ".com" - всего около 254 символов).
2. Нажать кнопку "Проверить".
   Ожидаемый результат: появляется alert с текстом "Прекрасный email-адрес".

Блок 4: Поведение при вводе

Название: "Ввод валидного email-адреса без нажатия кнопки "Проверить" "

Шаги воспроизведения:

1. Ввести адрес "user1517@inbox.ru" в поле для email.
2. Не нажимать кнопку "Проверить".
   Ожидаемый результат: cообщение об ошибке не отображается. Поле ввода просто содержит введенный текст. Валидация срабатывает исключительно по нажатию кнопки "Проверить".
