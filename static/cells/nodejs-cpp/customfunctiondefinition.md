##CustomFunctionDefinition
Definition of custom function for calculating with users custom engine.
## CustomFunctionDefinition class
Definition of custom function for calculating with user's custom engine.
```javascript
class CustomFunctionDefinition;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| abstract [getArrayModeParameters(string)](#getArrayModeParameters-string-)| Gets the indices of given custom function's parameters that need to be calculated in array mode. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### getArrayModeParameters(string) {#getArrayModeParameters-string-}
Gets the indices of given custom function's parameters that need to be calculated in array mode.
```javascript
abstract getArrayModeParameters(functionName: string) : number[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionName | string | Name of the custom function. |
**Returns**
Indices of the parameters that need to be calculated in array mode for given custom function. Default is null, there is no parameter which needs to be calculated in array mode for the custom function.
**Remarks**
For an expression that needs to be calculated, taking A:A+B:B as an example: Generally in value mode it will be calculated to a single value according to current cell base. But in array mode, all values of A1+B1,A2+B2,A3+B3,... will be calculated and used for the calculation.
