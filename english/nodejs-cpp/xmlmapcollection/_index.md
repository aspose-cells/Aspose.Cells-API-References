---
title: XmlMapCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: A collection of XmlMapnodejscppxmlmap objects that represent XmlMap information.
type: docs
url: /nodejs-cpp/xmlmapcollection/
---

## XmlMapCollection class

A collection of [XmlMap](/nodejs-cpp/xmlmap/) objects that represent XmlMap information.

```javascript
class XmlMapCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the xml map by the specific index. |
| [add(string)](#add-string-)| Add a [XmlMap](/nodejs-cpp/xmlmap/) by the url/path of a xml/xsd file. |
| [clear()](#clear--)| Removes all XmlMaps. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets the xml map by the specific index.

```javascript
get(index: number) : XmlMap;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

The xml map

### add(string) {#add-string-}

Add a [XmlMap](/nodejs-cpp/xmlmap/) by the url/path of a xml/xsd file.

```javascript
add(url: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| url | string | url/path of a xml/xsd file. |

**Returns**

[XmlMap](/nodejs-cpp/xmlmap/) object index.

### clear() {#clear--}

Removes all XmlMaps.

```javascript
clear() : void;
```


### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



