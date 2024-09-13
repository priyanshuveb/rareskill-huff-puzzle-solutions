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
#### offset
The offset is used to locate within the calldata where specific dynamic data starts or can be found.

#### quick lookup info
- ASCII values occupies 1 byte(2 hex char)
- 1 byte = 8 bits = 2 hex char
#### For more details on encoding please refer: [Reference](https://www.rareskills.io/post/abi-encoding)

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
- [SimulateArray] ❌
- [MyCreator] ✅
- [CountTime] ✅
- [TimeAndBlock] ✅


