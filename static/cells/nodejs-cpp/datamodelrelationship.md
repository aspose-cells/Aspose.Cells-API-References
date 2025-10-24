##DataModelRelationship
Represents a single relationship in the spreadsheet data model.
## DataModelRelationship class
Represents a single relationship in the spreadsheet data model.
```javascript
class DataModelRelationship;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [foreignKeyTable](#foreignKeyTable--)| string | Readonly. Gets the name of the foreign key table for this relationship. |
| [primaryKeyTable](#primaryKeyTable--)| string | Readonly. Gets the name of the primary key table for this relationship. |
| [foreignKeyColumn](#foreignKeyColumn--)| string | Readonly. Gets the name of the foreign key table column for this relationship. |
| [primaryKeyColumn](#primaryKeyColumn--)| string | Readonly. Gets the name of the primary key table column for this relationship. |
## Methods
| Method | Description |
| --- | --- |
| [getForeignKeyTable()](#getForeignKeyTable--)| <b>@deprecated.</b> Please use the 'foreignKeyTable' property instead. Gets the name of the foreign key table for this relationship. |
| [getPrimaryKeyTable()](#getPrimaryKeyTable--)| <b>@deprecated.</b> Please use the 'primaryKeyTable' property instead. Gets the name of the primary key table for this relationship. |
| [getForeignKeyColumn()](#getForeignKeyColumn--)| <b>@deprecated.</b> Please use the 'foreignKeyColumn' property instead. Gets the name of the foreign key table column for this relationship. |
| [getPrimaryKeyColumn()](#getPrimaryKeyColumn--)| <b>@deprecated.</b> Please use the 'primaryKeyColumn' property instead. Gets the name of the primary key table column for this relationship. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### foreignKeyTable {#foreignKeyTable--}
Readonly. Gets the name of the foreign key table for this relationship.
```javascript
foreignKeyTable : string;
```
### primaryKeyTable {#primaryKeyTable--}
Readonly. Gets the name of the primary key table for this relationship.
```javascript
primaryKeyTable : string;
```
### foreignKeyColumn {#foreignKeyColumn--}
Readonly. Gets the name of the foreign key table column for this relationship.
```javascript
foreignKeyColumn : string;
```
### primaryKeyColumn {#primaryKeyColumn--}
Readonly. Gets the name of the primary key table column for this relationship.
```javascript
primaryKeyColumn : string;
```
### getForeignKeyTable() {#getForeignKeyTable--}
```javascript
getForeignKeyTable() : string;
```
### getPrimaryKeyTable() {#getPrimaryKeyTable--}
```javascript
getPrimaryKeyTable() : string;
```
### getForeignKeyColumn() {#getForeignKeyColumn--}
```javascript
getForeignKeyColumn() : string;
```
### getPrimaryKeyColumn() {#getPrimaryKeyColumn--}
```javascript
getPrimaryKeyColumn() : string;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
