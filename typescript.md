### 1. 基本数据类型
   ```ts
   let a : number = 1;
   let str: string = 'abc';
  ```
### 2. 数组和元组
   let arr: number[] = [1, 2, 3];
   let arr2: [string, number] = ['string', 12];
### 3. 接口 interface
   interface home {
     readOnly id: number,
     name: string,
     age?: number
   }
### 4. 函数function
   function add(x: number, y: number): number {
	return x + y;
   }
   let result = add(1, 2);

  const add = (x: number, y: number, z?: number): number => {
    if(typeof z === 'number') {
     return x + y;
   }
  }
 
  interface ISum() {
    (x: number, y: number, z?: number): number
  }
  let add2: ISum = add;
### 5. union types
  let numberOrString: number | string;
  numberOrString.toString();
  
  const str = input as string;
  if(str.length) {
   return str.length;
  } else {
   const number = input as number;
   return number.toString().length;
 }

 function getLength2(input: string | number): number {
  if (typeof input === 'string') {
    return input.length;
  } else {
   return input.toString().length
 }
### 6. 类class
   static, public, private, protected, readonly
### 7. 类和 interface 继承
   interface Radio {
     switchRadio(trigger: boolean): void;
   }
   class car implements Radio {
   switchRadio(trigger: boolean): void {
   }
8. enum枚举  常量枚举 计算枚举
   enum Direction {
    up,
    down,
    left,
    right
   }

  const enum Direction{}
9. 泛型 generics
   function ech<T>(args: T): T {
     return arg
   }
   const result: string = echo('str');
10.约束泛型
   interface IWitchLength {
     length: number
   }

   function echoWithLength<T extends IWithLength>(arg: T): T {
     console.log(T.length);
     return T;
   }
11. 类型别名
    let sum: (x: number, y: nuber) => number;
    
   交叉类型
    type IPerson  = IName & { age: number };
12. declare var jQuer: (selector: string) => any;
13. 内置类型  
   
  
  
   
