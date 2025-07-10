---
title: DataModel
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the data model.
type: docs
url: /nodejs-cpp/datamodel/
---

## DataModel class

Represents the data model.

```javascript
class DataModel;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [relationships](#relationships--)| DataModelRelationshipCollection | Readonly. Gets all relationships of the tables in the data model. |
| [tables](#tables--)| DataModelTableCollection | Readonly. Gets all tables in the data model. |

## Methods

| Method | Description |
| --- | --- |
| [getRelationships()](#getRelationships--)| <b>@deprecated.</b> Please use the 'relationships' property instead. Gets all relationships of the tables in the data model. |
| [getTables()](#getTables--)| <b>@deprecated.</b> Please use the 'tables' property instead. Gets all tables in the data model. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### relationships {#relationships--}

Readonly. Gets all relationships of the tables in the data model.

```javascript
relationships : DataModelRelationshipCollection;
```


### tables {#tables--}

Readonly. Gets all tables in the data model.

```javascript
tables : DataModelTableCollection;
```


### getRelationships() {#getRelationships--}

<b>@deprecated.</b> Please use the 'relationships' property instead. Gets all relationships of the tables in the data model.

```javascript
getRelationships() : DataModelRelationshipCollection;
```


**Returns**

[DataModelRelationshipCollection](../datamodelrelationshipcollection/)

### getTables() {#getTables--}

<b>@deprecated.</b> Please use the 'tables' property instead. Gets all tables in the data model.

```javascript
getTables() : DataModelTableCollection;
```


**Returns**

[DataModelTableCollection](../datamodeltablecollection/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



