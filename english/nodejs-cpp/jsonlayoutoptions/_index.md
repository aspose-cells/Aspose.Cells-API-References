---
title: JsonLayoutOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options of json layout type.
type: docs
url: /nodejs-cpp/jsonlayoutoptions/
---

## JsonLayoutOptions class

Represents the options of json layout type.

```javascript
class JsonLayoutOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Constructor of loading JSON layout options. |

## Methods

| Method | Description |
| --- | --- |
| [getArrayAsTable()](#getArrayAsTable--)| Processes Array as table. |
| [setArrayAsTable(boolean)](#setArrayAsTable-boolean-)| Processes Array as table. |
| [getIgnoreNull()](#getIgnoreNull--)| Indicates whether ignoring null value. |
| [setIgnoreNull(boolean)](#setIgnoreNull-boolean-)| Indicates whether ignoring null value. |
| [getIgnoreTitle()](#getIgnoreTitle--)| Ingores titles of attributes |
| [setIgnoreTitle(boolean)](#setIgnoreTitle-boolean-)| Ingores titles of attributes |
| [getConvertNumericOrDate()](#getConvertNumericOrDate--)| Indicates whether converting the string in json to numeric or date value. |
| [setConvertNumericOrDate(boolean)](#setConvertNumericOrDate-boolean-)| Indicates whether converting the string in json to numeric or date value. |
| [get_NumberFormat()](#get_NumberFormat--)| Gets and sets the format of numeric value. |
| [setNumberFormat(string)](#setNumberFormat-string-)| Gets and sets the format of numeric value. |
| [get_DateFormat()](#get_DateFormat--)| Gets and sets the format of date value. |
| [setDateFormat(string)](#setDateFormat-string-)| Gets and sets the format of date value. |
| [getTitleStyle()](#getTitleStyle--)| Gets and sets the style of the title. |
| [setTitleStyle(Style)](#setTitleStyle-style-)| Gets and sets the style of the title. |
| [getKeptSchema()](#getKeptSchema--)| Indicates whether keeping schema of this json. |
| [setKeptSchema(boolean)](#setKeptSchema-boolean-)| Indicates whether keeping schema of this json. |


### constructor() {#constructor--}

Constructor of loading JSON layout options.

```javascript
constructor();
```


### getArrayAsTable() {#getArrayAsTable--}

Processes Array as table.

```javascript
getArrayAsTable() : boolean;
```


### setArrayAsTable(boolean) {#setArrayAsTable-boolean-}

Processes Array as table.

```javascript
setArrayAsTable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getIgnoreNull() {#getIgnoreNull--}

Indicates whether ignoring null value.

```javascript
getIgnoreNull() : boolean;
```


### setIgnoreNull(boolean) {#setIgnoreNull-boolean-}

Indicates whether ignoring null value.

```javascript
setIgnoreNull(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getIgnoreTitle() {#getIgnoreTitle--}

Ingores titles of attributes

```javascript
getIgnoreTitle() : boolean;
```


### setIgnoreTitle(boolean) {#setIgnoreTitle-boolean-}

Ingores titles of attributes

```javascript
setIgnoreTitle(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getConvertNumericOrDate() {#getConvertNumericOrDate--}

Indicates whether converting the string in json to numeric or date value.

```javascript
getConvertNumericOrDate() : boolean;
```


### setConvertNumericOrDate(boolean) {#setConvertNumericOrDate-boolean-}

Indicates whether converting the string in json to numeric or date value.

```javascript
setConvertNumericOrDate(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### get_NumberFormat() {#get_NumberFormat--}

Gets and sets the format of numeric value.

```javascript
get_NumberFormat() : string;
```


### setNumberFormat(string) {#setNumberFormat-string-}

Gets and sets the format of numeric value.

```javascript
setNumberFormat(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### get_DateFormat() {#get_DateFormat--}

Gets and sets the format of date value.

```javascript
get_DateFormat() : string;
```


### setDateFormat(string) {#setDateFormat-string-}

Gets and sets the format of date value.

```javascript
setDateFormat(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTitleStyle() {#getTitleStyle--}

Gets and sets the style of the title.

```javascript
getTitleStyle() : Style;
```


**Returns**

[Style](../style/)

### setTitleStyle(Style) {#setTitleStyle-style-}

Gets and sets the style of the title.

```javascript
setTitleStyle(value: Style) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](../style/) | The value to set. |

### getKeptSchema() {#getKeptSchema--}

Indicates whether keeping schema of this json.

```javascript
getKeptSchema() : boolean;
```


**Remarks**

Sometimes we will save the file to JSON after loading JSON file.

### setKeptSchema(boolean) {#setKeptSchema-boolean-}

Indicates whether keeping schema of this json.

```javascript
setKeptSchema(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Sometimes we will save the file to JSON after loading JSON file.


