## Код, который писала Котя

Файл с решениями, чтобы спустя какое-то время улыбнуться/ужаснуться/сравнить уровни тогда и сейчас или все вышеперечисленное.

А  еще этот код навечно останется таким и будет мучиться здесь до скончания времен! Буга-га!

### **Arguments Optional**
Задачка: [Arguments Optional](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/intermediate-algorithm-scripting/arguments-optional "Arguments Optional - freeCodeCamp")

Код лапками:
```js
function addTogether(a,b) {
  
  if (!Number.isInteger(a)){
    console.log('a не число, a = ' + a);
    return undefined;
  }
  else if(arguments.length > 1 && b === undefined){
    console.log('аргуметнов функции ' + arguments.length);
    return undefined;
  }

  else if (b === undefined){
 
          return function(b){
              if (!Number.isInteger(b)){
                console.log('b определено как не число. b= '+ b + ', тип данных= '+ typeof b);
                return undefined;
              } 
                  else if (Number.isInteger(b)){
                  console.log('Сложение с двумя парами скобок. Сумма= ' + (a+b));
                  return a+b;
            }            
    }
  }
        else if (Number.isInteger(a) && Number.isInteger(b)){
        console.log('Простое сложение чисел. Сумма= ' + (a+b));
        return a+b;
        }  
            else {
            console.log('Остальные случаи. Вернуть undefined');
            return undefined;               
            }
}

addTogether(5, undefined);
```
