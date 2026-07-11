---
title: PowerQueryFormulaItem
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the item of the power query formula.
type: docs
url: /nodejs-cpp/powerqueryformulaitem/
---

## PowerQueryFormulaItem class

Represents the item of the power query formula.

```javascript
class PowerQueryFormulaItem;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [name](#name--)| string | Readonly. Gets the name of the item. |
| [value](#value--)| string | Gets the value of the item. |
| [textValue](#textValue--)| string | Readonly. Gets the text value of the item. |
| [itemType](#itemType--)| PowerQueryFormulaItemType | Readonly. Gets the type of this item (Function, Parameter, List, Literal, or Unknown). |

## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the item. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Gets the value of the item. |
| [setValue(string)](#setValue-string-)| <b>@deprecated.</b> Please use the 'value' property instead. Gets the value of the item. |
| [getTextValue()](#getTextValue--)| <b>@deprecated.</b> Please use the 'textValue' property instead. Gets the text value of the item. |
| [getItemType()](#getItemType--)| <b>@deprecated.</b> Please use the 'itemType' property instead. Gets the type of this item (Function, Parameter, List, Literal, or Unknown). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### name {#name--}

Readonly. Gets the name of the item.

```javascript
name : string;
```


### value {#value--}

Gets the value of the item.

```javascript
value : string;
```


### textValue {#textValue--}

Readonly. Gets the text value of the item.

```javascript
textValue : string;
```


### itemType {#itemType--}

Readonly. Gets the type of this item (Function, Parameter, List, Literal, or Unknown).

```javascript
itemType : PowerQueryFormulaItemType;
```


### getName() {#getName--}

<b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the item.

```javascript
getName() : string;
```


### getValue() {#getValue--}

<b>@deprecated.</b> Please use the 'value' property instead. Gets the value of the item.

```javascript
getValue() : string;
```


### setValue(string) {#setValue-string-}

<b>@deprecated.</b> Please use the 'value' property instead. Gets the value of the item.

```javascript
setValue(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTextValue() {#getTextValue--}

<b>@deprecated.</b> Please use the 'textValue' property instead. Gets the text value of the item.

```javascript
getTextValue() : string;
```


### getItemType() {#getItemType--}

<b>@deprecated.</b> Please use the 'itemType' property instead. Gets the type of this item (Function, Parameter, List, Literal, or Unknown).

```javascript
getItemType() : PowerQueryFormulaItemType;
```


**Returns**

[PowerQueryFormulaItemType](../powerqueryformulaitemtype/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



