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
| [getDeleted()](#getDeleted--)| <b>@deprecated.</b> Please use the 'deleted' property instead. Indicates whether the smart tag is deleted. |
| [setDeleted(boolean)](#setDeleted-boolean-)| <b>@deprecated.</b> Please use the 'deleted' property instead. Indicates whether the smart tag is deleted. |
| [getProperties()](#getProperties--)| <b>@deprecated.</b> Please use the 'properties' property instead. Gets and set the properties of the smart tag. |
| [setProperties(SmartTagPropertyCollection)](#setProperties-smarttagpropertycollection-)| <b>@deprecated.</b> Please use the 'properties' property instead. Gets and set the properties of the smart tag. |
| [getUri()](#getUri--)| <b>@deprecated.</b> Please use the 'uri' property instead. Gets the namespace URI of the smart tag. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets the name of the smart tag. |
| [setLink(string, string)](#setLink-string-string-)| Change the name and  the namespace URI of the smart tag. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getDeleted() {#getDeleted--}
```javascript
getDeleted() : boolean;
```
### setDeleted(boolean) {#setDeleted-boolean-}
```javascript
setDeleted(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getProperties() {#getProperties--}
```javascript
getProperties() : SmartTagPropertyCollection;
```
**Returns**
[SmartTagPropertyCollection](../smarttagpropertycollection/)
### setProperties(SmartTagPropertyCollection) {#setProperties-smarttagpropertycollection-}
```javascript
setProperties(value: SmartTagPropertyCollection) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SmartTagPropertyCollection](../smarttagpropertycollection/) | The value to set. |
### getUri() {#getUri--}
```javascript
getUri() : string;
```
### getName() {#getName--}
```javascript
getName() : string;
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
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
