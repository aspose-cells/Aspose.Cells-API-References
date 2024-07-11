---
title: VbaModuleCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the list of [VbaModule](./vbamodule/)
type: docs
url: /nodejs-cpp/vbamodulecollection/
---

## VbaModuleCollection class

Represents the list of [VbaModule](./vbamodule/)

```javascript
class VbaModuleCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [VbaModule](./vbamodule/) in the list by the index. |
| [addDesignerStorage(string, number[])](#addDesignerStorage-string-number[]-)|  |
| [getDesignerStorage(string)](#getDesignerStorage-string-)| Represents the data of Designer. |
| [add(Worksheet)](#add-worksheet-)| Adds module for a worksheet. |
| [add(VbaModuleType, string)](#add-vbamoduletype-string-)| Adds module. |
| [addUserForm(string, string, number[])](#addUserForm-string-string-number[]-)| Inser user form into VBA Project. |
| [remove(Worksheet)](#remove-worksheet-)| Removes module for a worksheet. |
| [remove(string)](#remove-string-)| Remove the module by the name |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets [VbaModule](./vbamodule/) in the list by the index.

```javascript
get(index: number) : VbaModule;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

[VbaModule](./vbamodule/)

### addDesignerStorage(string, number[]) {#addDesignerStorage-string-number[]-}



```javascript
addDesignerStorage(name: string, data: number[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string |  |
| data | number[] |  |

### getDesignerStorage(string) {#getDesignerStorage-string-}

Represents the data of Designer.

```javascript
getDesignerStorage(name: string) : number[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string |  |

**Returns**

number[]

**Remarks**

We do not support to parse them. Just only for copying.

### add(Worksheet) {#add-worksheet-}

Adds module for a worksheet.

```javascript
add(sheet: Worksheet) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](./worksheet/) | The worksheet |

### add(VbaModuleType, string) {#add-vbamoduletype-string-}

Adds module.

```javascript
add(type: VbaModuleType, name: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [VbaModuleType](./vbamoduletype/) | The type of module. |
| name | string | The name of module. |

### addUserForm(string, string, number[]) {#addUserForm-string-string-number[]-}

Inser user form into VBA Project.

```javascript
addUserForm(name: string, codes: string, designerStorage: number[]) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of user form |
| codes | string | The codes for the user form |
| designerStorage | number[] | the designer setting about the user form |

### remove(Worksheet) {#remove-worksheet-}

Removes module for a worksheet.

```javascript
remove(sheet: Worksheet) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](./worksheet/) | The worksheet |

### remove(string) {#remove-string-}

Remove the module by the name

```javascript
remove(name: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string |  |

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



