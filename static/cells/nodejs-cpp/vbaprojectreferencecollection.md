##VbaProjectReferenceCollection
Represents all references of VBA project.
## VbaProjectReferenceCollection class
Represents all references of VBA project.
```javascript
class VbaProjectReferenceCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Get the reference in the list by the index. |
| [addRegisteredReference(string, string)](#addRegisteredReference-string-string-)| Add a reference to an Automation type library. |
| [addControlRefrernce(string, string, string, string)](#addControlRefrernce-string-string-string-string-)| Add a reference to a twiddled type library and its extended type library. |
| [addProjectRefrernce(string, string, string)](#addProjectRefrernce-string-string-string-)| Adds a reference to an external VBA project. |
| [copy(VbaProjectReferenceCollection)](#copy-vbaprojectreferencecollection-)| Copies references from other VBA project. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Get the reference in the list by the index.
```javascript
get(i: number) : VbaProjectReference;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| i | number | The index. |
**Returns**
[VbaProjectReference](../vbaprojectreference/)
### addRegisteredReference(string, string) {#addRegisteredReference-string-string-}
Add a reference to an Automation type library.
```javascript
addRegisteredReference(name: string, libid: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of reference. |
| libid | string | The identifier of an Automation type library. |
### addControlRefrernce(string, string, string, string) {#addControlRefrernce-string-string-string-string-}
Add a reference to a twiddled type library and its extended type library.
```javascript
addControlRefrernce(name: string, libid: string, twiddledlibid: string, extendedLibid: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of reference. |
| libid | string | The identifier of an Automation type library. |
| twiddledlibid | string | The identifier of a twiddled type library |
| extendedLibid | string | The identifier of an extended type library |
### addProjectRefrernce(string, string, string) {#addProjectRefrernce-string-string-string-}
Adds a reference to an external VBA project.
```javascript
addProjectRefrernce(name: string, absoluteLibid: string, relativeLibid: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of reference. |
| absoluteLibid | string | The referenced VBA project's identifier with an absolute path. |
| relativeLibid | string | The referenced VBA project's identifier with an relative path. |
### copy(VbaProjectReferenceCollection) {#copy-vbaprojectreferencecollection-}
Copies references from other VBA project.
```javascript
copy(source: VbaProjectReferenceCollection) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [VbaProjectReferenceCollection](../vbaprojectreferencecollection/) | The source references. |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
