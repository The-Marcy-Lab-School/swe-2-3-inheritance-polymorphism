# Short Responses

For this short response assignment, aim to write a response with the following qualities (your instructor will give you feedback on these areas):
- [] Addresses all parts of the prompt
- [] Accurately uses relevant technical terminology
- [] Is free of grammar and spelling mistakes (double check with grammarly!)
- [] Uses markdown to enhance readability (preview in VS Code with Command/Control + Shift + V)
- [] Is easy to comprehend

For each prompt below, write your response in the space provided. Aim to answer each prompt in 2-5 concise sentences. Make sure to preview your markdown to check how it is rendered before submitting.

## Prompt 1

Consider these classes:

```js
class Animal {
  eat() { return "eating"; }
}

class Dog extends Animal {
  bark() { return "woof"; }
}

class Puppy extends Dog {
  play() { return "playing"; }
}

const rex = new Puppy();
```

Explain what happens when `rex.eat()` is invoked. In your answer, describe the role of **inheritance** and the **prototype chain**.

## Response 1

--- 

## Prompt 2 

Look at these classes:

```js
class Employee {
  constructor(name, salary) {
    this.name = name;
    this.salary = salary;
  }
  getDetails() {
    return `${this.name} earns $${this.salary}`;
  }
}

class Manager extends Employee {
  constructor(name, salary, department) {
    // YOUR CODE HERE
  }
  getDetails() {
    // YOUR CODE HERE - should include both the Employee details 
    // AND the department info
  }
}
```

Complete the `Manager` class by filling in the `constructor` and `getDetails` methods. Explain why you need to use `super` in each method and what would happen if you didn't use it.

## Response 2

--- 

## Prompt 3

Examine this code:

```js
class Shape {
  constructor(type) {
    this.type = type;
  }
  getArea() {
    return 0;
  }
}

class Circle extends Shape {
  constructor(radius) {
    super('circle');
    this.radius = radius;
  }
  getArea() {
    return Math.PI * this.radius ** 2;
  }
}

class Square extends Shape {
  constructor(side) {
    super('square');
    this.side = side;
  }
  getArea() {
    return this.side ** 2;
  }
}

const shapes = [new Circle(5), new Square(4), new Circle(3)];
const totalArea = shapes.reduce((sum, shape) => sum + shape.getArea(), 0);
```

Explain how this code demonstrates **polymorphism**. Why can we call `getArea()` on each shape without checking what type of shape it is?

## Response 3
