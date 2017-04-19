# jspro
JavaScript Professional Course



№1
За допомогою каррінг створіть метод множення (mult) і 3 методи, які використовують його doubleNumber, tripleNumber, quartetNumber (повертає подвійну, утроенное і тд. Результат множення)


№2
Написати функцію, яка буде приймати массив елементів і рахувати суму цих елементів.

function sum() {
  function add (a, b) { return a + b; }
  return [].reduce.call(arguments, add);
}

№3
Написати фунцію, яка буде повертити ваше ім'я

function getName() { return this.name; }
getName();
// undefined

№4
Реалізувати метод, який за замовчуванням буде сумувати числа 1,2,3 (method()), а при інших параметрах буде сумувати їх з 1,2,3 (method(4,5)).
var calc = {
 add: function (a, b) { return a + b; },
 sum: function () { return [].reduce.call(arguments, this.add) }
};


Homework
№1
За домомогою медода apply знайдіть найбільший і найменший елемент
var myArray = [ 0, 10, 20, 'string', null, undefined, 100, 1  ];

№2
Перезапишіть код за допомогою ES6

var elements = [
  "Hydrogen",
  "Helium",
  "Lithium",
  "Beryllium"
];

var elements2 = elements.map(function(s){ return s.length });
var elements3 = elements.map(function(s){ return s.toUpperCase() });
var elements4 = elements.map(function(s){ return s.toLowerCase() });

№3
Створіть батьківський клас Product, який буде приймати 2 аргументи (назва і ціна).
 Усередині класу зробіть перевірку на випадок якщо ціна буде нижче 0
 в повідомленні виведіть ім'я товару і оповіщення про те що товар (ім'я товару)
 не можна створювати з негативною ціною. Також створіть 2 підкласи -
  Food і Toy які будуть наслідувати клас продукту, а також мати власну властивість (їжа та іграшка).
