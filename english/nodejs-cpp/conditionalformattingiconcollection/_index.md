---
title: ConditionalFormattingIconCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents  a collection of ConditionalFormattingIcon..conditionalformattingicon objects.
type: docs
url: /nodejs-cpp/conditionalformattingiconcollection/
---

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
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


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

**Remarks**

NOTE: This member is now obsolete. Instead, please use Add(IconSetType, int) method. This method will be removed 6 months later since December 2025. Aspose apologizes for any inconvenience you may have experienced.

### getCount() {#getCount--}

<b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



