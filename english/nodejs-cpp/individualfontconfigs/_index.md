---
title: IndividualFontConfigs
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Font configs for each Workbook..workbook object.
type: docs
url: /nodejs-cpp/individualfontconfigs/
---

## IndividualFontConfigs class

Font configs for each [Workbook](../workbook/) object.

```javascript
class IndividualFontConfigs;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Ctor. |

## Methods

| Method | Description |
| --- | --- |
| [setFontSubstitutes(string, string[])](#setFontSubstitutes-string-stringarray-)| Sets font substitute names for a given original font name. |
| [getFontSubstitutes(string)](#getFontSubstitutes-string-)| Returns an array containing font substitute names to be used if original font is not presented. |
| [setFontFolder(string, boolean)](#setFontFolder-string-boolean-)| Sets the fonts folder |
| [setFontFolders(string[], boolean)](#setFontFolders-stringarray-boolean-)| Sets the font folders |
| [setFontSources(FontSourceBase[])](#setFontSources-fontsourcebasearray-)| Sets the font sources. |
| [getFontSources()](#getFontSources--)| Gets a copy of the array that contains the list of sources |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Ctor.

```javascript
constructor();
```


### setFontSubstitutes(string, string[]) {#setFontSubstitutes-string-stringarray-}

Sets font substitute names for a given original font name.

```javascript
setFontSubstitutes(originalFontName: string, substituteFontNames: string[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | string | Original font name. |
| substituteFontNames | string[] | List of font substitute names to be used if original font is not presented. |

### getFontSubstitutes(string) {#getFontSubstitutes-string-}

Returns an array containing font substitute names to be used if original font is not presented.

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

Sets the font folders

```javascript
setFontFolders(fontFolders: string[], recursive: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolders | string[] | The folders that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |

### setFontSources(FontSourceBase[]) {#setFontSources-fontsourcebasearray-}

Sets the font sources.

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

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



