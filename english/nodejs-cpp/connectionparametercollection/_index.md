---
title: ConnectionParameterCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Specifies the ConnectionParameter..connectionparameter collection
type: docs
url: /nodejs-cpp/connectionparametercollection/
---

## ConnectionParameterCollection class

Specifies the [ConnectionParameter](../connectionparameter/) collection

```javascript
class ConnectionParameterCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [ConnectionParameter](../connectionparameter/) element at the specified index. |
| [get(string)](#get-string-)| Gets the [ConnectionParameter](../connectionparameter/) element with the specified name. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the [ConnectionParameter](../connectionparameter/) element at the specified index.

```javascript
get(index: number) : ConnectionParameter;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### get(string) {#get-string-}

Gets the [ConnectionParameter](../connectionparameter/) element with the specified name.

```javascript
get(connParamName: string) : ConnectionParameter;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| connParamName | string | connection parameter name |

**Returns**

The element with the specified name.

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



