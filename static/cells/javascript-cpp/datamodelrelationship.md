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
