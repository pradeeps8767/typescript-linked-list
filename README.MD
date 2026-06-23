# TypeScript Linked List

A simple implementation of a generic singly linked list in TypeScript.

## Features

- Generic implementation using TypeScript generics (`LinkedList<T>`)
- Add elements to the end of the list
- Keep track of the number of elements
- Print all elements in the list
- Supports any data type

## Project Structure

```
.
├── linked-list.ts
└── README.md
```

## Implementation

### `ListNode<T>`

Represents a node in the linked list.

```ts
class ListNode<T> {
  next?: ListNode<T>;

  constructor(public value: T) {}
}
```

### `LinkedList<T>`

Represents a generic singly linked list.

#### Methods

| Method | Description |
|----------|-------------|
| `add(value)` | Adds a new element to the end of the list |
| `getNumberOfElements()` | Returns the number of elements in the list |
| `print()` | Prints all elements in the list |

## Example

```ts
const numberList = new LinkedList<number>();

numberList.add(11);
numberList.add(20);
numberList.add(5);

console.log(numberList.getNumberOfElements());

numberList.print();
```

Output:

```text
3
11
20
5
```

### Using with Strings

```ts
const nameList = new LinkedList<string>();

nameList.add("John");
nameList.add("Jane");

console.log(nameList.getNumberOfElements());

nameList.print();
```

Output:

```text
2
John
Jane
```

## Running the Project

### Install TypeScript

```bash
npm install
```

### Compile

```bash
tsc linked-list.ts
```

### Watch Mode

```bash
tsc --watch
```

### Run

```bash
node linked-list.js
```

## Future Improvements

- [ ] Insert at beginning
- [ ] Insert at a specific position
- [ ] Delete by value
- [ ] Delete by index
- [ ] Search for an element
- [ ] Reverse the linked list
- [ ] Convert linked list to array
- [ ] Support iteration
- [ ] Doubly linked list implementation

## Technologies

- TypeScript
- Node.js
