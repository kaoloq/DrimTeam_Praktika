## DrimTeam_Praktika
Команда: Кушкоева Анастасия, Давкаева Валентина, Судакова Полина

# Спецификация программы поразрядной сортировки RadixSort
  **Постановка задачи**
  Программа должна выполнять сортировку элементов типа Integer и String поразрядным методом и осуществлять визуализацию работы данного алгоритма. Она должна обладать графическим интерфейсом пользователя (GUI) с возможностью ручного ввода элементов для сортировки.
  **Описание алгоритма и структуры данных**
  Алгоритм предназначен для сортировки целых чисел, записанных цифрами. Но так как в памяти компьютеров любая информация записывается целыми числами, алгоритм пригоден для сортировки любых объектов, запись которых можно поделить на «разряды», содержащие сравнимые значения. Сортировать можно не только числа, записанные в виде набора цифр, но и строки, являющиеся набором символов, и вообще произвольные значения в памяти, представленные в виде набора байт.
Сравнение производится поразрядно: сначала сравниваются значения одного крайнего разряда, и элементы группируются по результатам этого сравнения, затем сравниваются значения следующего разряда, соседнего, и элементы либо упорядочиваются по результатам сравнения значений этого разряда внутри образованных на предыдущем проходе групп, либо переупорядочиваются в целом, но сохраняя относительный порядок, достигнутый при предыдущей сортировке. Затем аналогично делается для следующего разряда, и так до конца.
  Данная программа будет состоять из двух базовых классов:
    · класс, отвечающий за GUI и обеспечивающий работу основной логики программы;
    · класс, реализующий разработку алгоритма поразрядной сортировки.
  **Формат входных и выходных данных**
    · Integer
    · String
  **Описание GUI**
    Для визуализации перемещения элементов по колонкам, текущий сортируемый элемент визуально выносится за пределы массива и имеет более крупный размер шрифта для отображения. На следующем шаге он переносится в нужную колонку, которая в свою очередь выделяется цветом. При этом, на его место встает следующий элемент рабочего массива.
    
