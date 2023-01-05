Basic types in TypeScript: TypeScript has several basic types, including boolean, number, and string. It also has a void type, which is used to represent the absence of a return value for a function. Additionally, TypeScript has a null and undefined type, which can be used to represent the absence of a value.

- Interfaces: In TypeScript, an interface is a way to define a contract for the shape of an object. You can use interfaces to define the structure of an object, including the names and types of its properties and methods. 
For example:

```
interface Point {
  x: number;
  y: number;
}
```
- Classes: TypeScript has classes, which are a way to define a blueprint for an object. You can use classes to define the properties and methods that an object will have, as well as to define its constructor function. 

For example:
```
class Point {
  constructor(public x: number, public y: number) {}

  distanceFromOrigin() {
    return Math.sqrt(this.x * this.x + this.y * this.y);
  }
}
```
- Functions: TypeScript has functions, which are blocks of code that can be called by name. You can define the parameters and return type of a function using TypeScript's type annotations. For example:
```
function add(x: number, y: number): number {
  return x + y;
}
```
- Working with the DOM and TypeScript: To work with the DOM (Document Object Model) in TypeScript, you can use the Document interface provided by the TypeScript standard library. This interface provides a way to access and modify DOM elements and events. 

For example:

```
const button = document.querySelector('button');
button.addEventListener('click', () => console.log('Clicked!'));
Generic types: TypeScript has generic types, which allow you to define a type that can be customized with other types. You can use generic types to create reusable types that work with a variety of different data types. For example:

function identity<T>(arg: T): T {
  return arg;
}
```

- Namespaces: In TypeScript, a namespace is a way to organize your code into logical groups. You can use namespaces to prevent naming conflicts and to create a hierarchy of types. For example:

```
namespace Shapes {
  export class Circle { ... }
  export class Square { ... }
}
```

Merging declarations: In TypeScript, you can use the declare keyword to merge multiple declarations into a single definition. This can be useful when working with third-party libraries that don't have their own TypeScript declarations. 

For example:
```
// foo.d.ts
declare module "foo" {
  export function bar(): void;
}

// baz.ts
import * as foo from "foo";
foo.bar();
``` 
- Ambient namespaces: An ambient namespace is a way to include declarations for a third-party library in your TypeScript code. You can use ambient namespaces to tell the TypeScript compiler about the types and values that are available in a library, without actually including the library's


