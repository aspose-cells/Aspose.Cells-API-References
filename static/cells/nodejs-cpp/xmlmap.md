##XmlMap
Represents Xml map information.
## XmlMap class
Represents Xml map information.
```javascript
class XmlMap;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [name](#name--)| string | Returns or sets the name of the object. |
| [rootElementName](#rootElementName--)| string | Readonly. Gets root element name. |
| [dataBinding](#dataBinding--)| XmlDataBinding | Readonly. Gets an [XmlDataBinding](../xmldatabinding/) of this map. |
## Methods
| Method | Description |
| --- | --- |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Returns or sets the name of the object. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Returns or sets the name of the object. |
| [getRootElementName()](#getRootElementName--)| <b>@deprecated.</b> Please use the 'rootElementName' property instead. Gets root element name. |
| [getDataBinding()](#getDataBinding--)| <b>@deprecated.</b> Please use the 'dataBinding' property instead. Gets an [XmlDataBinding](../xmldatabinding/) of this map. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### name {#name--}
Returns or sets the name of the object.
```javascript
name : string;
```
### rootElementName {#rootElementName--}
Readonly. Gets root element name.
```javascript
rootElementName : string;
```
### dataBinding {#dataBinding--}
Readonly. Gets an [XmlDataBinding](../xmldatabinding/) of this map.
```javascript
dataBinding : XmlDataBinding;
```
### getName() {#getName--}
```javascript
getName() : string;
```
### setName(string) {#setName-string-}
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getRootElementName() {#getRootElementName--}
```javascript
getRootElementName() : string;
```
### getDataBinding() {#getDataBinding--}
```javascript
getDataBinding() : XmlDataBinding;
```
**Returns**
[XmlDataBinding](../xmldatabinding/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
