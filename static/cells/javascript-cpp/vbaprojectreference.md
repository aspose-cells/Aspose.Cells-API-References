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
| [copy(VbaProjectReference)](#copy-vbaprojectreference-)|  |
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
### copy(VbaProjectReference) {#copy-vbaprojectreference-}
```javascript
copy(source: VbaProjectReference) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [VbaProjectReference](../vbaprojectreference/) |  |
