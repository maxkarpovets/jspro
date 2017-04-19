### JavaScript Professional Course

# №1

var elements = [
  "Hydrogen",
  "Helium",
  "Lithium",
  "Beryllium"
];

var elements2 = elements.map(function(s){ return s.length });
var elements3 = elements.map(function(s){ return s.toUpperCase() });
var elements4 = elements.map(function(s){ return s.toLowerCase() });


# №2

Написати функцію, яка буде приймати массив елементів і рахувати суму цих елементів.

function sum() {
  function add (a, b) { return a + b; }
  return [].reduce.call(arguments, add);
}

# №3

Написати фунцію, яка буде повертити ваше ім'я

function getName() { return this.name; }
getName();
// undefined

# №4

Реалізувати метод, який за замовчуванням буде сумувати числа 1,2,3 (method()), а при інших параметрах буде сумувати їх з 1,2,3 (method(4,5)).
var calc = {
 add: function (a, b) { return a + b; },
 sum: function () { return [].reduce.call(arguments, this.add) }
};

# 4
Реалізувати вивід чисел від 0 до 9 за допомогою данного методу

for(var i = 0; i < 10; i++) {
    setTimeout(function() {
      console.log(i);  
    }, 10);
}

# №5

Реалізувати метод doSomething так, щоб він виводив ваше ім'я, і щоб його можна було виводити лише через даний метод
var MyModule = (function() {
  var name = 'Max';
  function sayHello() {
      console.log('Hello ' + name.toUpperCase());
 }
 
  //Here;
 }
})();
MyModule.doSomething();

#  №6

Є 3 герої: Хан, Дарт, Люк.
Вивести їх повні імена за домопогою метода map
## Homework

# №1
За домомогою медода apply знайдіть найбільший і найменший елемент
var myArray = [ 0, 10, 20, 'string', null, undefined, 100, 1  ];

# №2

Створіть метод множення (mult) і 3 методи, які використовують його doubleNumber, tripleNumber, quartetNumber (повертає подвійну, потрійне і тд. результат множення)
Перезапишіть код за допомогою ES6

# №3
Створіть батьківський клас Product, який буде приймати 2 аргументи (назва і ціна).
 Усередині класу зробіть перевірку на випадок якщо ціна буде нижче 0
 в повідомленні виведіть ім'я товару і оповіщення про те що товар (ім'я товару)
 не можна створювати з негативною ціною. Також створіть 2 підкласи -
  Food і Toy які будуть наслідувати клас продукту, а також мати власну властивість (їжа та іграшка).

# №4
Визначити злих персонажів за допомогою методів map i filter.

function Person(name, side) {
    this.name = name;
    this.side = side;
}

var hanSolo = new Person('Han Solo','Rebels');
var bobaFett = new Person('Darth Vader','Empire');
var princessLeia = new Person('Princess Leia', 'Rebels');
