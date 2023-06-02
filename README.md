## МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ РОССИЙСКОЙ ФЕДЕРАЦИИ ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»<br>
Лабораторная работа №12<br>
"JS"<br>

Выполнил: Акимов И.В.<br>

Проверил: Соболев Е. И.<br>

г. Южно-Сахалинск<br>
2023 год<br>

#### Введениe<br>
Решение задач на php.<br>
Цели и задачи<br>
1.	Создайте массив, заполненный числами от 1 до 100. Найдите сумму элементов данного массива.

         $num = range(1, 100);  
         echo array_sum($num);

2.	Дан массив с элементами 'a', 'b', 'c', 'd', 'e'. С помощью функции array_map сделайте из него массив 'A', 'B', 'C', 'D', 'E'.

          $arr = array('a', 'b', 'c', 'd', 'e');
          $new_arr = array_map('strtoupper', $arr);
          print_r($new_arr)."\n";


3.	Дан массив $arr. Подсчитайте количество элементов этого массива.

         $arr = range(1, 2, 3, 4, 5);  
         echo count($arr);

4.	Дан массив $arr. С помощью функции count выведите последний элемент данного массива.

          $arr = [1, 2, 3, 4];
          echo $arr[count($arr) - 1];

5.	Дан массив с числами. Проверьте, что в нем есть элемент со значением 3.

   
         $arr = [1, 2, 2, 4];
        var_dump(in_array(3, $arr));

6.	Дан массив [1, 2, 3, 4, 5]. Найдите сумму элементов данного массива.

           $num = range(1, 2, 3, 4, 5);  
         echo array_sum($num);

7.	Дан массив [1, 2, 3, 4, 5]. Найдите произведение (умножение) элементов данного массива.

          $arr = [1, 2, 3, 4, 5];
          echo array_product($arr);

8.	Дан массив $arr. С помощью функций array_sum и count найдите среднее арифметическое элементов (сумма элементов делить на их количество) данного массива.
                
                $arr = [1, 2, 3, 4, 5];
            echo array_sum($arr) / count($arr);

                
9.	Создайте массив, заполненный числами от 1 до 100.
  
          $num = range(1, 100); 

10	Создайте массив, заполненный буквами от 'a' до 'z'.

          $az = range('a', 'z');

11	 Создайте строку '1-2-3-4-5-6-7-8-9' не используя цикл.

          $arr = range(1, 9);
          $arr1 = implode('-', $arr);
          echo $arr1;

12	Найдите сумму чисел от 1 до 100 не используя цикл.

           $num = range(1, 100);  
           echo array_sum($num);

13	 Найдите произведение чисел от 1 до 10 не используя цикл.

           $arr = range(1, 100); 
           echo array_product($arr);

14	Даны два массива: первый с элементами 1, 2, 3, второй с элементами 'a', 'b', 'c'. Сделайте из них массив с элементами 1, 2, 3, 'a', 'b', 'c'.

            $num = [1, 2, 3];
            $az = ['a', 'b', 'c'];
           $array = array_merge($num, $az);
           print_r($array);
            
15	Дан массив с элементами 1, 2, 3, 4, 5. С помощью функции array_slice создайте из него массив $result с элементами 2, 3, 4.

        $arr=array(1, 2, 3, 4, 5);
        $result = array_slice($arr, 1, 3);
        print_r($result)."\n";

16	Дан массив [1, 2, 3, 4, 5]. С помощью функции array_splice преобразуйте массив в [1, 4, 5].

         $arr=array(1, 2, 3, 4, 5);
        $result = array_slice($arr, 1, 2);
        print_r($result)."\n";

17	 Дан массив [1, 2, 3, 4, 5]. С помощью функции array_splice запишите в новый массив элементы [2, 3, 4].

        $arr = [1, 2, 3, 4, 5];
        var_dump(array_splice($arr, 0, 1));
        var_dump(array_splice($arr, 2, 2));

18	 Дан массив [1, 2, 3, 4, 5]. С помощью функции array_splice сделайте из него массив [1, 2, 3, 'a', 'b', 'c', 4, 5].

        $arr = [1, 2, 3, 4, 5];
        var_dump(array_splice($arr, 3, 0, ['a', 'b', 'c']));

19	 Дан массив [1, 2, 3, 4, 5]. С помощью функции array_splice сделайте из него массив [1, 'a', 'b', 2, 3, 4, 'c', 5, 'e'].

        $arr = [1, 2, 3, 4, 5];
        $arr = array_splice($arr, 1, 0, ['a', 'b']);
        $arr = array_splice($arr, 6, 0, ['c']);
        $arr = array_splice($arr, 8, 0, ['e']);

20.	 Дан массив 'a'=>1, 'b'=>2, 'c'=>3'. Запишите в массив $keys ключи из этого массива, а в $values – значения.

          $arr = ['a'=>1, 'b'=>2, 'c'=>3];
         $keys = array_keys($arr);
         $values = array_values($arr);
         print_r($keys)."\n";
          print_r($values)."\n";

21.	 Даны два массива: ['a', 'b', 'c'] и [1, 2, 3]. Создайте с их помощью массив 'a'=>1, 'b'=>2, 'c'=>3'.

          $arr1 = ['a', 'b', 'c'];
          $arr2 = [1, 2, 3];
          var_dump(array_combine($arr1, $arr2));

22.	Дан массив 'a'=>1, 'b'=>2, 'c'=>3. Поменяйте в нем местами ключи и значения.

        $arr = ['a'=>1, 'b'=>2, 'c'=>3];
        var_dump(array_flip($arr));

23.	 Дан массив с элементами 1, 2, 3, 4, 5. Сделайте из него массив с элементами 5, 4, 3, 2, 1.

          var_dump(array_reverse([1, 2, 3, 4, 5]));

24.	Дан массив ['a', '-', 'b', '-', 'c', '-', 'd']. Найдите позицию первого элемента '-'.

        $arr =  ['a', '-', 'b', '-', 'c', '-', 'd'];
        $pos = array_search('-', $arr);

25.	 Дан массив ['a', '-', 'b', '-', 'c', '-', 'd']. Найдите позицию первого элемента '-' и удалите его с помощью функции array_splice.
 
           $arr =  ['a', '-', 'b', '-', 'c', '-', 'd'];
                 $pos = array_search('-', $arr);
          var_dump(array_splice($arr, $pos, 1));

26.	Дан массив ['a', 'b', 'c', 'd', 'e']. Поменяйте элемент с ключом 0 на '!', а элемент с ключом 3 - на '!!'.

          $arr =  ['a', 'b', 'c', 'd', 'e'];
          var_dump(array_replace($arr, [0 => '!', 3 => '!!']));

27.	Дан массив '3'=>'a', '1'=>'c', '2'=>'e', '4'=>'b'. Попробуйте на нем различные типы сортировок.

        $arr = ['3'=>'a', '1'=>'c', '2'=>'e', '4'=>'b'];
        var_dump(sort($arr)); // по возрастанию элементов
        var_dump(rsort($arr)); // по убыванию элементов
        var_dump(ksort($arr)); // по возрастанию ключей
        var_dump(krsort($arr)); // по убыванию ключей

28.	Дан массив с элементами 'a'=>1, 'b'=>2, 'c'=>3. Выведите на экран случайный ключ из данного массива.

        $arr = ['a'=>1, 'b'=>2, 'c'=>3];
        echo array_rand($arr);

29.	 Дан массив с элементами 'a'=>1, 'b'=>2, 'c'=>3. Выведите на экран случайный элемент данного массива.

          $arr = ['a'=>1, 'b'=>2, 'c'=>3];        
          echo $arr[array_rand($arr)];

30.	Дан массив $arr. Перемешайте его элементы в случайном порядке.

        $arr = [1, 2, 3, 4, 5];
        var_dump(shuffle($arr));

31.	 Заполните массив числами от 1 до 25 с помощью range, а затем перемешайте его элементы в случайном порядке.

    $num = shuffle(range(1, 25));

32.	 Создайте массив, заполненный буквами от 'a' до 'z' так, чтобы буквы шли в случайном порядке и не повторялись.

    $az = shuffle(range('a', 'z'));

33.	 Сделайте строку длиной 6 символов, состоящую из маленьких английских букв, расположенных в случайном порядке. Буквы не должны повторяться.

          $arr = range('a', 'z');
          shuffle($arr);
          echo implode('', array_slice(0, 6));

34.	Дан массив с элементами 'a', 'b', 'c', 'b', 'a'. Удалите из него повторяющиеся элементы.

        $az = ['a', 'b', 'c', 'b', 'a'];
        var_dump(array_unique($az));  

35.	Дан массив с элементами 1, 2, 3, 4, 5. Выведите на экран его первый и последний элемент, причем так, чтобы в исходном массиве они исчезли.

        $arr = [1, 2, 3, 4, 5];
        echo array_shift($arr);
        echo array_pop($arr);

36.	 Дан массив с элементами 1, 2, 3, 4, 5. Добавьте ему в начало элемент 0, а в конец - элемент 6.

          $arr = [1, 2, 3, 4, 5];
          array_unshift($arr,0);
          array_push($arr, 6);

37.	 Дан массив с элементами 1, 2, 3, 4, 5, 6, 7, 8. С помощью цикла и функций array_shift и array_pop выведите на экран его элементы в следующем порядке: 18273645. 

          $arr = [1, 2, 3, 4, 5, 6, 7, 8];
          $str = '';
          while (!empty($arr)) {
              $str .= array_shift($arr);
              $str .= array_pop($arr);
          }
          echo $str;

38.	 Дан массив с элементами 'a', 'b', 'c'. Сделайте из него массив с элементами 'a', 'b', 'c', '-', '-', '-'.

          $arr = ['a', 'b', 'c'];
          $new = array_pad($arr, 6, '-'); 

39.	 Заполните массив 10-ю буквами 'x'.

          $arr = array_fill(0, 10, 'x');

40.	 Создайте массив, заполненный целыми числами от 1 до 20. С помощью функции array_chunk разбейте этот массив на 5 подмассивов ([1, 2, 3, 4]; [5, 6, 7, 8] и т.д.).

          $arr = range(1, 20);
          $arr = array_chunk($arr, 4);

#### Вывод<br>
научился работь с массивами и использовать функции
