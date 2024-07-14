---
title: AutoNumberedBulletValue
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents automatic numbered bullet.
type: docs
url: /nodejs-cpp/autonumberedbulletvalue/
---

## AutoNumberedBulletValue class

Represents automatic numbered bullet.

```javascript
class AutoNumberedBulletValue extends BulletValue;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(BulletValue)](#constructor-bulletvalue-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of the bullet. |
| [getStartAt()](#getStartAt--)| Gets and sets the starting number of the bullet. |
| [setStartAt(number)](#setStartAt-number-)| Gets and sets the starting number of the bullet. |
| [getAutonumberScheme()](#getAutonumberScheme--)| Represents the scheme of automatic number. |
| [setAutonumberScheme(TextAutonumberScheme)](#setAutonumberScheme-textautonumberscheme-)| Represents the scheme of automatic number. |


### constructor(BulletValue) {#constructor-bulletvalue-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: BulletValue);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | BulletValue | The parent object. |

### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getType() {#getType--}

Gets the type of the bullet.

```javascript
getType() : BulletType;
```


**Returns**

[BulletType](/nodejs-cpp/bullettype/)

### getStartAt() {#getStartAt--}

Gets and sets the starting number of the bullet.

```javascript
getStartAt() : number;
```


### setStartAt(number) {#setStartAt-number-}

Gets and sets the starting number of the bullet.

```javascript
setStartAt(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getAutonumberScheme() {#getAutonumberScheme--}

Represents the scheme of automatic number.

```javascript
getAutonumberScheme() : TextAutonumberScheme;
```


**Returns**

[TextAutonumberScheme](/nodejs-cpp/textautonumberscheme/)

### setAutonumberScheme(TextAutonumberScheme) {#setAutonumberScheme-textautonumberscheme-}

Represents the scheme of automatic number.

```javascript
setAutonumberScheme(value: TextAutonumberScheme) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAutonumberScheme](/nodejs-cpp/textautonumberscheme/) | The value to set. |


