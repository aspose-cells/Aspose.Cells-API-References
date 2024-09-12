---
title: ScenarioCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the list of scenarios.
type: docs
url: /nodejs-cpp/scenariocollection/
---

## ScenarioCollection class

Represents the list of scenarios.

```javascript
class ScenarioCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Scenario](../scenario/) object by the index. |
| [getActiveIndex()](#getActiveIndex--)| Gets and sets which scenario is selected. |
| [setActiveIndex(number)](#setActiveIndex-number-)| Gets and sets which scenario is selected. |
| [getLastSelected()](#getLastSelected--)| Indicates which scenario was last selected by the user to be run/shown. |
| [setLastSelected(number)](#setLastSelected-number-)| Indicates which scenario was last selected by the user to be run/shown. |
| [add(string)](#add-string-)| Adds a scenario. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the [Scenario](../scenario/) object by the index.

```javascript
get(index: number) : Scenario;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The specific index in the list. |

**Returns**

[Scenario](../scenario/)

### getActiveIndex() {#getActiveIndex--}

Gets and sets which scenario is selected.

```javascript
getActiveIndex() : number;
```


### setActiveIndex(number) {#setActiveIndex-number-}

Gets and sets which scenario is selected.

```javascript
setActiveIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLastSelected() {#getLastSelected--}

Indicates which scenario was last selected by the user to be run/shown.

```javascript
getLastSelected() : number;
```


### setLastSelected(number) {#setLastSelected-number-}

Indicates which scenario was last selected by the user to be run/shown.

```javascript
setLastSelected(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### add(string) {#add-string-}

Adds a scenario.

```javascript
add(name: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of scenario. |

**Returns**

The index in the list of scenarios.

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



