---
title: WebExtensionReferenceCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the list of web extension reference.
type: docs
url: /nodejs-cpp/webextensionreferencecollection/
---

## WebExtensionReferenceCollection class

Represents the list of web extension reference.

```javascript
class WebExtensionReferenceCollection implements Iterable<WebExtensionReference>;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets web extension by the specific index. |
| [add()](#add--)| Adds an empty reference of web extension. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |

## \[Symbol.iterator\](): Iterator\<WebExtensionReference\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### get(number) {#get-number-}

Gets web extension by the specific index.

```javascript
get(index: number) : WebExtensionReference;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

The web extension

### add() {#add--}

Adds an empty reference of web extension.

```javascript
add() : number;
```


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



