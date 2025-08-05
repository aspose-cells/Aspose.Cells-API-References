---
title: PictureBulletValue
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the value of the image bullet.
type: docs
url: /js-cpp/picturebulletvalue/
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

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [imageData](#imageData--)| Uint8Array | Gets and sets image data of the bullet. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of the bullet's value. |


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


### imageData {#imageData--}

Gets and sets image data of the bullet.

```javascript
imageData : Uint8Array;
```


### getType() {#getType--}

Gets the type of the bullet's value.

```javascript
getType() : BulletType;
```


**Returns**

[BulletType](../bullettype/)


