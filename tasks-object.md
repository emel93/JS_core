Задачки для работы с объектами

1) isPlainObject. Напишите функцию, которая проверяет, является ли элемент именно простым объектом, а не массивом, null и т.п.MakePairs. Напишите функцию, которая возвращает вложенный массив вида [[key, value], [key, value]].
/**
  * Описание задачи: Напишите функцию, которая возвращает вложенный массив вида `[[key, value], [key, value]]`.
  * Ожидаемый результат: ({ a: 1, b: 2 }) => [['a', 1], ['b', 2]]
  * Сложность задачи: 1 of 5
  * @param {Object} object - любой объект для трансформации
  * @returns {Array} - вложенный массив
*/

export const makePairs = (object) => {
  throw new Error(`Напишите здесь свое решение ${object}`);
};

const data = { a: 1, b: 2 };
console.log(makePairs(data)); // [['a', 1], ['b', 2]]
/**
  * Описание задачи: Напишите функцию, которая проверяет, является ли элемент именно простым объектом, а не массивом, null и т.п.
  * Ожидаемый результат: true если это объект, false в противном случае. ({ a: 1 }) => true, ([1, 2, 3]) => false
  * @param element - элемент для проверки
  * @returns {boolean}
*/

export const isPlainObject = (element) => {
  throw new Error(`Напишите здесь свое решение ${element}`);
};

const data = { a: 1 };
console.log(isPlainObject(data)); // true


2) MakePairs. Напишите функцию, которая возвращает вложенный массив вида [[key, value], [key, value]].
/**
  * Описание задачи: Напишите функцию, которая возвращает вложенный массив вида `[[key, value], [key, value]]`.
  * Ожидаемый результат: ({ a: 1, b: 2 }) => [['a', 1], ['b', 2]]
  * @param {Object} object - любой объект для трансформации
  * @returns {Array} - вложенный массив
*/

export const makePairs = (object) => {
  throw new Error(`Напишите здесь свое решение ${object}`);
};

const data = { a: 1, b: 2 };
console.log(makePairs(data)); // [['a', 1], ['b', 2]]

3) Without. Напишите функцию, которая возвращает новый объект без указанных значений.
/**
  * Описание задачи: Напишите функцию, которая возвращает новый объект без указанных значений.
  * Ожидаемый результат: ({ a: 1, b: 2 }, 'b') => { a: 1 }
  * @param {Object} object - любой объект
  * @param {?} args - список значений для удаления
  * @returns {Object} - новый объект без удаленных значений
*/

export const without = (object, ...args) => {
  throw new Error(`Напишите здесь свое решение ${object} ${args}`);
};

const data = { a: 1, b: 2, c: 3 };
console.log(without(data, 'b', 'c')); // { a: 1 }

4) IsEmpty. Напишите функцию, которая делает поверхностную проверку объекта на пустоту.
/**
  * Описание задачи: Напишите функцию, которая делает поверхностную проверку объекта на пустоту.
  * Ожидаемый результат: ({}) => true,
      ({ a: undefined }) => true,
      ({ a: 1 }) => false
  * Пустые значения: '', null, NaN, undefined
  * @param {Object} object - объект с примитивами
  * @returns {boolean}
*/

export const isEmpty = (object) => {
  throw new Error(`Напишите здесь свое решение ${object}`);
};

const data = { a: 1, b: undefined };
const data2 = { a: undefined };
console.log(isEmpty(data)); // false
console.log(isEmpty(data2)); // true

5) IsEqual. Напишите функцию, которая поверхностно сравнивает два объекта.
/**
  * Описание задачи: Напишите функцию, которая поверхностно сравнивает два объекта.
  * Ожидаемый результат: True если объекты идентичны, false если объекты разные ({ a: 1, b: 1 }, { a: 1, b: 1 }) => true
  * @param {Object<string | number>} firstObj - объект с примитивами
  * @param {Object<string | number>} secondObj - объект с примитивами
  * @returns {boolean}
*/

export const isEqual = (firstObject, secondObject) => {
  throw new Error(`Напишите здесь свое решение ${firstObject} ${secondObject}`);
};

const data = { a: 1, b: 1 };
const data2 = { a: 1, b: 1 };
const data3 = { a: 1, b: 2 };
console.log(isEqual(data, data2)); // true
console.log(isEqual(data, data3)); // false

6) Invoke. Напишите функцию, которая вызывает метод массива на заданный путь объекта.
/**
  * Описание задачи: Напишите функцию, которая вызывает метод массива на заданный путь объекта.
  * Ожидаемый результат: ({ a: { b: [1, 2, 3] } }, 'a.b', splice, [1, 2]) => [2, 3]
  * @param {Object} object
  * @param {String} path - путь в объекте
  * @param {String} func - метод массива для исполнения
  * @param {Array} [args] - список аргументов
  * @returns {?}
*/

export const invoke = (object, path, func, args) => {
  throw new Error(`Напишите здесь свое решение ${object} ${path} ${func} ${args}`);
};

const data = { a: { b: [1, 2, 3] } }
console.log(invoke(data, 'a.b', 'splice', [1, 2])); // [2, 3]

7) IsEmptyDeep. Напишите функцию, которая делает глубокую проверку на пустоту объекта.
/**
  * Описание задачи: Напишите функцию, которая делает глубокую проверку на пустоту объекта.
  * Пустые значения: '', null, NaN, undefined, [], {}
  * Ожидаемый результат: ({}) => true,
      ({ a: { b: undefined } }) => true,
      ({ a: { b: [] } }) => true
  * @param {Object} object - любой объект
  * @returns {boolean}
*/

export const isEmptyDeep = (object) => {
  throw new Error(`Напишите здесь свое решение ${object}`);
};

const data = { a: { b: undefined } };
const data2 = { a: { b: 1 } };
console.log(isEmptyDeep(data)); // true
console.log(isEmptyDeep(data2)); // false

8) IsEqualDeep. Напишите функцию, которая делает глубокое сравнение объектов.
/**
  * Описание задачи: Напишите функцию, которая делает глубокое сравнение объектов.
  * Ожидаемый результат: True если объекты идентичны ({ a: 1, b: { c: 1 } }, { a: 1, b: { c: 1 } }) => true
  * @param {Object} firstObj - Объект с любыми значениями
  * @param {Object} secondObj - Объект с любыми значениями
  * @returns {boolean}
*/
export const isEqualDeep = (element) => {
  throw new Error(`Напишите здесь свое решение ${element}`);
};
const data = { a: 1, b: { c: 1 } };
const data2 = { a: 1, b: { c: 1 } };
const data3 = { a: 1, b: { c: 2 } };
console.log(isEqualDeep(data, data2)); // true
console.log(isEqualDeep(data, data3)); // false

9) Intersection. Напишите функцию, которая поверхностно находит пересечения объектов и возвращает объект пересечений.
/**
  * Описание задачи: Напишите функцию, которая поверхностно находит пересечения объектов и возвращает объект пересечений.
  * Ожидаемый результат: ({ a: 1, b: 2 }, { c: 1, b: 2 }) => { b: 2 }
  * @param {Object<string | number>} firstObj - объект с примитивными значениями
  * @param {Object<string | number>} secondObj - объект с примитивными значениями
  * @returns {Object}
*/

export const intersection = (firstObject, secondObject) => {
  throw new Error(`Напишите здесь свое решение ${firstObject}, ${secondObject}`);
};

const data = { a: 1, b: 2 };
const data2 = { c: 1, b: 2 };
console.log(intersection(data, data2)); // { b: 2 }

10) IntersectionDeep. Напишите функцию, которая глубоко находит пересечения объектов и возвращает объект пересечений.
/**
  * Описание задачи: Напишите функцию, которая глубоко находит пересечения объектов и возвращает объект пересечений.
  * Ожидаемый результат: ({ a: 1, b: { c: 3 } }, { c: 1, b: { c: 3 } }) => { b: { c: 3 } }
  * @param {Object} firstObj - объект любых значений
  * @param {Object} secondObj - объект любых значений
  * @returns {Object}
*/

export const intersectionDeep = (firstObject, secondObject) => {
  throw new Error(`Напишите здесь свое решение ${firstObject}, ${secondObject}`);
};

const data = { a: 1, b: { c: 3 } };
const data2 = { c: 1, b: { c: 3 } };
console.log(intersectionDeep(data, data2)); // { b: { c: 3 } }
