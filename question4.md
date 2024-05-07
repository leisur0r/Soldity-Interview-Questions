### 4. What are the major changes to arithmetic operations in Solidity version 0.8.0?
Answer:From Solidity 0.8.0, arithmetic operations are rolled back on underflows and overflows. This means that if the result of an arithmetic operation is outside the range of its data type, the operation will fail and be rolled back. Before Solidity 0.8.0, 
integer underflows and overflows are allowed without causing errors. To avoid this, Solidity 0.8.0 has arithmetic operation checking enabled by default. If you need to use old arithmetic operations, you can use unchecked{... } statement block
