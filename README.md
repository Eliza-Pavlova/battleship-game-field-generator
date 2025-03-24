# Генератор поля игры "Морской бой"

Этот скрипт на Python генерирует поля для игры "Морской бой". Он позволяет случайным образом размещать корабли на игровом поле, поддерживает сохранение и загрузку уже существующих игровых полей из файлов.

## Особенности

- **Размеры полей**: поддерживает сетки 5x5, 6x6, 7x7, 8x8, 9x9 и 10x10.
- **Случайное размещение кораблей**: корабли размещаются автоматически программой без наложений кораблей друг на друга или непосредственного соседства кораблей.
- **Сохранение/Загрузка**: сохраняйте поле в файл и загрузите его позже.
- **Отображение поля**: выводит текущее игровое поле с координатами.

## Требования

- Python 3.x

## Как пользоваться кодом

1. **Запустите скрипт**: запустите программу, затем выберите размер поля или загрузите поле из файла.
2. **Размещение кораблей**: корабли размещаются случайным образом на выбранной сетке.
3. **Сохранение/Загрузка**: сохраните поле в файл или загрузите ранее сохраненное поле.

## Функции

- create_field(size): создает пустое игровое поле заданного размера.
- print_field(field): отображает игровое поле с координатами строк и столбцов.
- can_place_ship(field, start_row, start_col, end_row, end_col): проверяет, можно ли разместить корабль на поле по указанным координатам.
- place_ship(field, start_row, start_col, end_row, end_col): размещает корабль на поле по указанным координатам.
- mark_surroundings(field, start_row, start_col, end_row, end_col): помечает окружающие клетки как недоступные для размещения кораблей.
- setup_ships(field, ships): случайным образом размещает корабли на поле в соответствии с заданной конфигурацией.
- save_field_to_file(field): сохраняет текущее игровое поле в файл (game_field.txt).
- load_field_from_file(filename="game_field.txt"): загружает игровое поле из указанного файла.
- valid_input(prompt, min_value, max_value): запрашивает у пользователя ввод до тех пор, пока не будет введено допустимое число в заданном диапазоне.
- main(): основная функция, управляющая логикой игры, включающая выбор поля, размещение кораблей, сохранение и загрузку.
