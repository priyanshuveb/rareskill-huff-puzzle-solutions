## Prerequisites
#### Data Type and their encoding
  - Static data:
    - bool
    - uints
    - bytes on fixed size (bytesN)
    - address
    - struct with fixed data
    - fixed size array
  - Dynamic data:
    - bytes
    - string
    - dynamic array
    - a fixed-size array with any above dynamic type data
    - a struct that contains any of the above dynamic types
  - The staic data type are padded left in the encoding whereas the dynamic types are padded right
  - While encoding dynamic types an additional value `offset`, size are included in encoding. Dynamic encoding is special
#### Offset
The offset is used to locate within the calldata where specific dynamic data starts or can be found.

#### Quick lookup info
- ASCII values occupies 1 byte(2 hex char)
- 1 byte = 8 bits = 2 hex char
- [evm.codes for opcode references](https://www.evm.codes/?fork=cancun)
- [evm.playground for analysing the bytecode](https://www.evm.codes/playground?fork=shanghai)
## Links: 
- [Reference for detailed overview on encoding](https://www.rareskills.io/post/abi-encoding)
- [Rareskill Huff Puzzle Repo](https://github.com/RareSkills/huff-puzzles/tree/main)
- [Pre written huff contracts for complex data structure and tokens that can be imported](https://github.com/huff-language/huffmate/tree/main/src)

## Setup

Get Huff
```bash
curl -L get.huff.sh | bash
huffup
```

Compile huff code to get the bytecode if needed 
```bash
huffc ./src/fileName.huff -b
```

Installation
```bash
git clone https://github.com/priyanshuveb/rareskill-huff-puzzle-solutions.git
cd rareskill-huff-puzzle-solutions
forge install
```
To run a test
```bash
forge test -v --mc CallValue
```

## Exercises
- [CallValue] ✅
- [CalldataLength] ✅
- [MyEtherBalance] ✅
- [Add1] ✅
- [Multiply] ✅
- [NonPayable] ✅
- [FooBar] ✅
- [SimpleStore] ✅
- [RevertCustom] ✅
- [RevertString] ✅
- [SumArray] ✅
- [Keccak] ✅
- [MaxOfArray] ✅
- [Create] ✅
- [Emitter] ✅
- [Donations] ✅
- [SendEther] ✅
- [BasicBank] ✅
- [Distribute] ✅
- [SimulateArray] ✅
- [MyCreator] ✅
- [CountTime] ✅
- [TimeAndBlock] ✅


