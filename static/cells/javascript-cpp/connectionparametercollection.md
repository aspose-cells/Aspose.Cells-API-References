##ConnectionParameterCollection
Specifies the ConnectionParameter..connectionparameter collection
## ConnectionParameterCollection class
Specifies the [ConnectionParameter](../connectionparameter/) collection
```javascript
class ConnectionParameterCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [ConnectionParameter](../connectionparameter/) element at the specified index. |
| [get(string)](#get-string-)| Gets the [ConnectionParameter](../connectionparameter/) element with the specified name. |
| [set(ConnectionParameter, number)](#set-connectionparameter-number-)| Gets the [ConnectionParameter](../connectionparameter/) element at the specified index. |
### get(number) {#get-number-}
Gets the [ConnectionParameter](../connectionparameter/) element at the specified index.
```javascript
get(index: number) : ConnectionParameter;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### get(string) {#get-string-}
Gets the [ConnectionParameter](../connectionparameter/) element with the specified name.
```javascript
get(connParamName: string) : ConnectionParameter;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| connParamName | string | connection parameter name |
**Returns**
The element with the specified name.
### set(ConnectionParameter, number) {#set-connectionparameter-number-}
Gets the [ConnectionParameter](../connectionparameter/) element at the specified index.
```javascript
set(value: ConnectionParameter, index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ConnectionParameter](../connectionparameter/) |  |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
