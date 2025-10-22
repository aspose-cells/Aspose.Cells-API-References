##VbaProjectReference
Represents the reference of VBA project.
## VbaProjectReference class
Represents the reference of VBA project.
```javascript
class VbaProjectReference;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| VbaProjectReferenceType | Readonly. Gets the type of this reference. |
| [name](#name--)| string | Gets and sets the name of the reference. |
| [libid](#libid--)| string | Gets and sets the Libid of the reference. |
| [twiddledlibid](#twiddledlibid--)| string | Gets and sets the twiddled Libid of the reference. |
| [extendedLibid](#extendedLibid--)| string | Gets and sets the extended Libid of the reference. |
| [relativeLibid](#relativeLibid--)| string | Gets and sets the referenced VBA project's identifier with an relative path. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets the type of this reference. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the reference. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the reference. |
| [getLibid()](#getLibid--)| <b>@deprecated.</b> Please use the 'libid' property instead. Gets and sets the Libid of the reference. |
| [setLibid(string)](#setLibid-string-)| <b>@deprecated.</b> Please use the 'libid' property instead. Gets and sets the Libid of the reference. |
| [getTwiddledlibid()](#getTwiddledlibid--)| <b>@deprecated.</b> Please use the 'twiddledlibid' property instead. Gets and sets the twiddled Libid of the reference. |
| [setTwiddledlibid(string)](#setTwiddledlibid-string-)| <b>@deprecated.</b> Please use the 'twiddledlibid' property instead. Gets and sets the twiddled Libid of the reference. |
| [getExtendedLibid()](#getExtendedLibid--)| <b>@deprecated.</b> Please use the 'extendedLibid' property instead. Gets and sets the extended Libid of the reference. |
| [setExtendedLibid(string)](#setExtendedLibid-string-)| <b>@deprecated.</b> Please use the 'extendedLibid' property instead. Gets and sets the extended Libid of the reference. |
| [getRelativeLibid()](#getRelativeLibid--)| <b>@deprecated.</b> Please use the 'relativeLibid' property instead. Gets and sets the referenced VBA project's identifier with an relative path. |
| [setRelativeLibid(string)](#setRelativeLibid-string-)| <b>@deprecated.</b> Please use the 'relativeLibid' property instead. Gets and sets the referenced VBA project's identifier with an relative path. |
| [copy(VbaProjectReference)](#copy-vbaprojectreference-)|  |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### type {#type--}
Readonly. Gets the type of this reference.
```javascript
type : VbaProjectReferenceType;
```
### name {#name--}
Gets and sets the name of the reference.
```javascript
name : string;
```
### libid {#libid--}
Gets and sets the Libid of the reference.
```javascript
libid : string;
```
### twiddledlibid {#twiddledlibid--}
Gets and sets the twiddled Libid of the reference.
```javascript
twiddledlibid : string;
```
**Remarks**
Only for control reference.
### extendedLibid {#extendedLibid--}
Gets and sets the extended Libid of the reference.
```javascript
extendedLibid : string;
```
**Remarks**
Only for control reference.
### relativeLibid {#relativeLibid--}
Gets and sets the referenced VBA project's identifier with an relative path.
```javascript
relativeLibid : string;
```
**Remarks**
Only for project reference.
### getType() {#getType--}
```javascript
getType() : VbaProjectReferenceType;
```
**Returns**
[VbaProjectReferenceType](../vbaprojectreferencetype/)
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
### getLibid() {#getLibid--}
```javascript
getLibid() : string;
```
### setLibid(string) {#setLibid-string-}
```javascript
setLibid(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getTwiddledlibid() {#getTwiddledlibid--}
```javascript
getTwiddledlibid() : string;
```
**Remarks**
Only for control reference.
### setTwiddledlibid(string) {#setTwiddledlibid-string-}
```javascript
setTwiddledlibid(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
Only for control reference.
### getExtendedLibid() {#getExtendedLibid--}
```javascript
getExtendedLibid() : string;
```
**Remarks**
Only for control reference.
### setExtendedLibid(string) {#setExtendedLibid-string-}
```javascript
setExtendedLibid(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
Only for control reference.
### getRelativeLibid() {#getRelativeLibid--}
```javascript
getRelativeLibid() : string;
```
**Remarks**
Only for project reference.
### setRelativeLibid(string) {#setRelativeLibid-string-}
```javascript
setRelativeLibid(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
Only for project reference.
### copy(VbaProjectReference) {#copy-vbaprojectreference-}
```javascript
copy(source: VbaProjectReference) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [VbaProjectReference](../vbaprojectreference/) |  |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
