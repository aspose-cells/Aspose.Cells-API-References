##IndividualFontConfigs
Font configs for each Workbook..workbook object.
## IndividualFontConfigs class
Font configs for each [Workbook](../workbook/) object.
```javascript
class IndividualFontConfigs;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Ctor. |
## Methods
| Method | Description |
| --- | --- |
| [setFontSubstitutes(string, string[])](#setFontSubstitutes-string-stringarray-)| Font substitute names for given original font name. |
| [getFontSubstitutes(string)](#getFontSubstitutes-string-)| Returns array containing font substitute names to be used if original font is not presented. |
| [setFontFolder(string, boolean)](#setFontFolder-string-boolean-)| Sets the fonts folder |
| [setFontFolders(string[], boolean)](#setFontFolders-stringarray-boolean-)| Sets the fonts folders |
| [setFontSources(FontSourceBase[])](#setFontSources-fontsourcebasearray-)| Sets the fonts sources. |
| [getFontSources()](#getFontSources--)| Gets a copy of the array that contains the list of sources |
### constructor() {#constructor--}
Ctor.
```javascript
constructor();
```
### setFontSubstitutes(string, string[]) {#setFontSubstitutes-string-stringarray-}
Font substitute names for given original font name.
```javascript
setFontSubstitutes(originalFontName: string, substituteFontNames: string[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | string | Original font name. |
| substituteFontNames | string[] | List of font substitute names to be used if original font is not presented. |
### getFontSubstitutes(string) {#getFontSubstitutes-string-}
Returns array containing font substitute names to be used if original font is not presented.
```javascript
getFontSubstitutes(originalFontName: string) : string[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | string | originalFontName |
**Returns**
An array containing font substitute names to be used if original font is not presented.
### setFontFolder(string, boolean) {#setFontFolder-string-boolean-}
Sets the fonts folder
```javascript
setFontFolder(fontFolder: string, recursive: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolder | string | The folder that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |
### setFontFolders(string[], boolean) {#setFontFolders-stringarray-boolean-}
Sets the fonts folders
```javascript
setFontFolders(fontFolders: string[], recursive: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolders | string[] | The folders that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |
### setFontSources(FontSourceBase[]) {#setFontSources-fontsourcebasearray-}
Sets the fonts sources.
```javascript
setFontSources(sources: FontSourceBase[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sources | [FontSourceBase](../fontsourcebase/)[] | An array of sources that contain TrueType fonts. |
### getFontSources() {#getFontSources--}
Gets a copy of the array that contains the list of sources
```javascript
getFontSources() : FontSourceBase[];
```
**Returns**
[FontSourceBase](../fontsourcebase/)[]
