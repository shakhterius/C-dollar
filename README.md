Инструкция по применению компилятора и виртуальной машины C$ (Си-доллар).
-
Язык программирования ```С$``` был придуман в целях написания сценариев (особенно хорошее применение найдёт в геймдеве).
Можно рассматривать как альтернативу и замену – Pawn (устаревший и малофункциональный) с Lua (не Си-подобный).
В остальном имеется много всяких годных плюшек, которых нет в том же Pawn/Lua и прочих скриптовых языках.

Для исходных кодов на ```C$``` используется расширение (формат) файл|а(ов) – `cdlr`, для откомпилированных файл|а(ов) – `bccdlr` <br><br>
Точка выполнения скрипта начинается с создания основной функции. Есть два стандартных подхода к этому: <br>

1]: придумываем любое название для функции (обычно не применяется на практике);<br>
2]: название для функции соответствует имени файла (часто применимо на практике);<br>
<br>
В обоих случаях расположение функции должно быть в самом начале скрипта. <br>

| Вариант | Исходный код: |
|---------|---------------|

| № | на английском | на русском |
|---------|---------------|------------|
| ```1``` | ```1``` ```function ExecuteScript(){}```       | ```1``` ```функция ВыполнитьСкрипт(){}```     |
| ```2``` | ```1``` ```function ScriptEntryPoint(){}```    | ```1``` ```функция точкаВходаВскрипт(){}```   |
| ```3``` | ```1``` ```function Script(){}```              | ```1``` ```функция Скрипт(){}```              |
| ```4``` | ```1``` ```function 0(){}```                   | ```1``` ```функция 0(){}```                    |
<br>
Исходя из того, что функции выполняют какие-либо действия, то и названия у них должны быть соответствующие. На мой взгляд, первый вариант можно считать самым подходящим.<br>
<br>
Вызовем функцию не имеющую названия (безымянная).<br><br>

< файл: ```0.cdlr``` ><br>
``` 1 | 0(){} ```<br>
<br>
< файл: ```0.bccdlr``` ><br>
``` ```

Данная конструкция пустая и делать ничего не будет.<br>

<br>
<br>

---------------------
* Продолжение следует
---------------------
