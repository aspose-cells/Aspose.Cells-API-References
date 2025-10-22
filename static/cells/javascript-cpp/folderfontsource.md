##FolderFontSource
Represents the folder that contains TrueType font files.
## FolderFontSource class
Represents the folder that contains TrueType font files.
```javascript
class FolderFontSource extends FontSourceBase;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(FontSourceBase)](#constructor-fontsourcebase-)| Constructs from a parent object convertible to this. |
| [constructor(string, boolean)](#constructor-string-boolean-)| Ctor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [folderPath](#folderPath--)| string | Readonly. Path to fonts folder. |
| [scanSubFolders](#scanSubFolders--)| boolean | Readonly. Determines whether or not to scan the subfolders. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| Returns the type of the font source. |
### constructor(FontSourceBase) {#constructor-fontsourcebase-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: FontSourceBase);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | FontSourceBase | The parent object. |
### constructor(string, boolean) {#constructor-string-boolean-}
Ctor.
```javascript
constructor(folderPath: string, scanSubfolders: boolean);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| folderPath | string | path to fonts folder |
| scanSubfolders | boolean | Determines whether or not to scan subfolders. |
### folderPath {#folderPath--}
Readonly. Path to fonts folder.
```javascript
folderPath : string;
```
### scanSubFolders {#scanSubFolders--}
Readonly. Determines whether or not to scan the subfolders.
```javascript
scanSubFolders : boolean;
```
### getType() {#getType--}
Returns the type of the font source.
```javascript
getType() : FontSourceType;
```
**Returns**
[FontSourceType](../fontsourcetype/)
