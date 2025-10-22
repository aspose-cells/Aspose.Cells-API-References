##ConditionalFormattingIconCollection
Represents  a collection of ConditionalFormattingIcon..conditionalformattingicon objects.
## ConditionalFormattingIconCollection class
Represents  a collection of [ConditionalFormattingIcon](../conditionalformattingicon/) objects.
```javascript
class ConditionalFormattingIconCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the ConditionalFormattingIcon element at the specified index. |
| [add(IconSetType, number)](#add-iconsettype-number-)| Adds [ConditionalFormattingIcon](../conditionalformattingicon/) object. |
| [add(ConditionalFormattingIcon)](#add-conditionalformattingicon-)| Adds [ConditionalFormattingIcon](../conditionalformattingicon/) object. |
### get(number) {#get-number-}
Gets the ConditionalFormattingIcon element at the specified index.
```javascript
get(index: number) : ConditionalFormattingIcon;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### add(IconSetType, number) {#add-iconsettype-number-}
Adds [ConditionalFormattingIcon](../conditionalformattingicon/) object.
```javascript
add(type: IconSetType, index: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [IconSetType](../iconsettype/) | The value type. |
| index | number | The Index. |
**Returns**
Returns the index of new object in the list.
### add(ConditionalFormattingIcon) {#add-conditionalformattingicon-}
Adds [ConditionalFormattingIcon](../conditionalformattingicon/) object.
```javascript
add(cficon: ConditionalFormattingIcon) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cficon | [ConditionalFormattingIcon](../conditionalformattingicon/) | Returns the index of new object in the list. |
