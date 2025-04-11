---
title: PictureBulletValue
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the value of the image bullet.
type: docs
url: /nodejs-cpp/picturebulletvalue/
---

## PictureBulletValue class

Represents the value of the image bullet.

```javascript
class PictureBulletValue extends BulletValue;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(BulletValue)](#constructor-bulletvalue-)| Constructs from a parent object convertible to this. |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of the bullet's value. |
| [getImageData()](#getImageData--)| Gets and sets image data of the bullet. |
| [setImageData(Uint8Array)](#setImageData-uint8array-)| Gets and sets image data of the bullet. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


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

Gets the type of the bullet's value.

```javascript
getType() : BulletType;
```


**Returns**

[BulletType](../bullettype/)

### getImageData() {#getImageData--}

Gets and sets image data of the bullet.

```javascript
getImageData() : Uint8Array;
```


### setImageData(Uint8Array) {#setImageData-uint8array-}

Gets and sets image data of the bullet.

```javascript
setImageData(value: Uint8Array) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



