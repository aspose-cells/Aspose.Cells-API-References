---
title: ExternalConnectionCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Specifies the ExternalConnection..externalconnection collection
type: docs
url: /javascript-cpp/externalconnectioncollection/
---

## ExternalConnectionCollection class

Specifies the [ExternalConnection](../externalconnection/) collection

```javascript
class ExternalConnectionCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [ExternalConnection](../externalconnection/) element at the specified index. |
| [get(string)](#get-string-)| Gets the [ExternalConnection](../externalconnection/) element with the specified name. |
| [getExternalConnectionById(number)](#getExternalConnectionById-number-)| Gets the [ExternalConnection](../externalconnection/) element with the specified id. |


### get(number) {#get-number-}

Gets the [ExternalConnection](../externalconnection/) element at the specified index.

```javascript
get(index: number) : ExternalConnection;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### get(string) {#get-string-}

Gets the [ExternalConnection](../externalconnection/) element with the specified name.

```javascript
get(connectionName: string) : ExternalConnection;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| connectionName | string | the name of data connection |

**Returns**

The element with the specified name.

### getExternalConnectionById(number) {#getExternalConnectionById-number-}

Gets the [ExternalConnection](../externalconnection/) element with the specified id.

```javascript
getExternalConnectionById(connId: number) : ExternalConnection;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| connId | number | external connection id |

**Returns**

The element with the specified id.


