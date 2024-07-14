---
title: ConditionalFormattingValueCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Describes a collection of CFValueObject. Use only for icon sets.
type: docs
url: /nodejs-cpp/conditionalformattingvaluecollection/
---

## ConditionalFormattingValueCollection class

Describes a collection of CFValueObject. Use only for icon sets.

```javascript
class ConditionalFormattingValueCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Get the CFValueObject element at the specified index. |
| [add(FormatConditionValueType, string)](#add-formatconditionvaluetype-string-)| Adds [ConditionalFormattingValue](/nodejs-cpp/conditionalformattingvalue/) object. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Get the CFValueObject element at the specified index.

```javascript
get(index: number) : ConditionalFormattingValue;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### add(FormatConditionValueType, string) {#add-formatconditionvaluetype-string-}

Adds [ConditionalFormattingValue](/nodejs-cpp/conditionalformattingvalue/) object.

```javascript
add(type: FormatConditionValueType, value: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [FormatConditionValueType](/nodejs-cpp/formatconditionvaluetype/) | The value type. |
| value | string | The value. |

**Returns**

Returns the index of new object in the list.

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



