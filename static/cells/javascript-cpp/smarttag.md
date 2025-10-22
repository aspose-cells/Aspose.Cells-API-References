##SmartTag
Represents a smart tag.
## SmartTag class
Represents a smart tag.
```javascript
class SmartTag;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [deleted](#deleted--)| boolean | Indicates whether the smart tag is deleted. |
| [properties](#properties--)| SmartTagPropertyCollection | Gets and set the properties of the smart tag. |
| [uri](#uri--)| string | Readonly. Gets the namespace URI of the smart tag. |
| [name](#name--)| string | Readonly. Gets the name of the smart tag. |
## Methods
| Method | Description |
| --- | --- |
| [setLink(string, string)](#setLink-string-string-)| Change the name and  the namespace URI of the smart tag. |
### deleted {#deleted--}
Indicates whether the smart tag is deleted.
```javascript
deleted : boolean;
```
### properties {#properties--}
Gets and set the properties of the smart tag.
```javascript
properties : SmartTagPropertyCollection;
```
### uri {#uri--}
Readonly. Gets the namespace URI of the smart tag.
```javascript
uri : string;
```
### name {#name--}
Readonly. Gets the name of the smart tag.
```javascript
name : string;
```
### setLink(string, string) {#setLink-string-string-}
Change the name and  the namespace URI of the smart tag.
```javascript
setLink(uri: string, name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uri | string | The namespace URI of the smart tag. |
| name | string | The name of the smart tag. |
