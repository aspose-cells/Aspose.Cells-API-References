---
title: HtmlTableLoadOptionCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the table options when importing HTML.
type: docs
url: /javascript-cpp/htmltableloadoptioncollection/
---

## HtmlTableLoadOptionCollection class

Represents the table options when importing HTML.

```javascript
class HtmlTableLoadOptionCollection;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [tableToListObject](#tableToListObject--)| boolean | Indicates whether generate list objects from imported tables. The default value is false. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [HtmlTableLoadOption](../htmltableloadoption/) element at the specified index. |
| [add(HtmlTableLoadOption)](#add-htmltableloadoption-)| Adds one HtmlTableLoadOption into this collection. |
| [add(number)](#add-number-)| Add a HtmlTableLoadOption to the list. |
| [add(string)](#add-string-)| Add a HtmlTableLoadOption to the list. |
| [add(number, number)](#add-number-number-)| Add a HtmlTableLoadOption to the list. |
| [add(string, number)](#add-string-number-)| Add a HtmlTableLoadOption to the list. |
| [add(number, number, number)](#add-number-number-number-)| Add a HtmlTableLoadOption to the list. |
| [add(string, number, number)](#add-string-number-number-)| Add a HtmlTableLoadOption to the list. |
| [addTableLoadOption(HtmlTableLoadOption)](#addTableLoadOption-htmltableloadoption-)| Adds one HtmlTableLoadOption into this collection. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### tableToListObject {#tableToListObject--}

Indicates whether generate list objects from imported tables. The default value is false.

```javascript
tableToListObject : boolean;
```


### get(number) {#get-number-}

Gets the [HtmlTableLoadOption](../htmltableloadoption/) element at the specified index.

```javascript
get(index: number) : HtmlTableLoadOption;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### add(HtmlTableLoadOption) {#add-htmltableloadoption-}

Adds one HtmlTableLoadOption into this collection.

```javascript
add(item: HtmlTableLoadOption) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [HtmlTableLoadOption](../htmltableloadoption/) | one HtmlTableLoadOption |

**Returns**

the index of the added item

**Remarks**

NOTE: This member is now obsolete. Instead, please use AddTableLoadOption() method. This method will be removed 6 months later since December 2025. Aspose apologizes for any inconvenience you may have experienced.

### add(number) {#add-number-}

Add a HtmlTableLoadOption to the list.

```javascript
add(tableIndex: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tableIndex | number | Table index |

### add(string) {#add-string-}

Add a HtmlTableLoadOption to the list.

```javascript
add(tableId: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tableId | string | Table ID |

### add(number, number) {#add-number-number-}

Add a HtmlTableLoadOption to the list.

```javascript
add(tableIndex: number, targetSheetIndex: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tableIndex | number | Table index |
| targetSheetIndex | number | The target index of worksheet in Excel |

### add(string, number) {#add-string-number-}

Add a HtmlTableLoadOption to the list.

```javascript
add(tableId: string, targetSheetIndex: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tableId | string | Table ID |
| targetSheetIndex | number | The target index of worksheet in Excel |

### add(number, number, number) {#add-number-number-number-}

Add a HtmlTableLoadOption to the list.

```javascript
add(tableIndex: number, targetSheetIndex: number, originalSheetIndex: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tableIndex | number | Table index |
| targetSheetIndex | number | The target index of worksheet in Excel |
| originalSheetIndex | number | The original index of worksheet in the html |

### add(string, number, number) {#add-string-number-number-}

Add a HtmlTableLoadOption to the list.

```javascript
add(tableId: string, targetSheetIndex: number, originalSheetIndex: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tableId | string | Table ID |
| targetSheetIndex | number | The target index of worksheet in Excel |
| originalSheetIndex | number | The original index of worksheet in the html |

### addTableLoadOption(HtmlTableLoadOption) {#addTableLoadOption-htmltableloadoption-}

Adds one HtmlTableLoadOption into this collection.

```javascript
addTableLoadOption(item: HtmlTableLoadOption) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [HtmlTableLoadOption](../htmltableloadoption/) | one HtmlTableLoadOption |

**Returns**

the index of the added item


