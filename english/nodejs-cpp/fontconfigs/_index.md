---
title: FontConfigs
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Specifies font settings
type: docs
url: /nodejs-cpp/fontconfigs/
---

## FontConfigs class

Specifies font settings

```javascript
class FontConfigs;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| static [getDefaultFontName()](#getDefaultFontName--)| Gets or sets the default font name. |
| static [setDefaultFontName(string)](#setDefaultFontName-string-)| Gets or sets the default font name. |
| static [getPreferSystemFontSubstitutes()](#getPreferSystemFontSubstitutes--)| Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false. |
| static [setPreferSystemFontSubstitutes(boolean)](#setPreferSystemFontSubstitutes-boolean-)| Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false. |
| static [isFontAvailable(string)](#isFontAvailable-string-)| Indicate whether the font is available. |
| static [setFontSubstitutes(string, string[])](#setFontSubstitutes-string-stringarray-)| Font substitute names for given original font name. |
| static [getFontSubstitutes(string)](#getFontSubstitutes-string-)| Returns array containing font substitute names to be used if original font is not presented. |
| static [setFontFolder(string, boolean)](#setFontFolder-string-boolean-)| Sets the fonts folder |
| static [setFontFolders(string[], boolean)](#setFontFolders-stringarray-boolean-)| Sets the fonts folders |
| static [setFontSources(FontSourceBase[])](#setFontSources-fontsourcebasearray-)| Sets the fonts sources. |
| static [getFontSources()](#getFontSources--)| Gets a copy of the array that contains the list of sources |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getDefaultFontName() {#getDefaultFontName--}

Gets or sets the default font name.

```javascript
static getDefaultFontName() : string;
```


### setDefaultFontName(string) {#setDefaultFontName-string-}

Gets or sets the default font name.

```javascript
static setDefaultFontName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPreferSystemFontSubstitutes() {#getPreferSystemFontSubstitutes--}

Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false.

```javascript
static getPreferSystemFontSubstitutes() : boolean;
```


### setPreferSystemFontSubstitutes(boolean) {#setPreferSystemFontSubstitutes-boolean-}

Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false.

```javascript
static setPreferSystemFontSubstitutes(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isFontAvailable(string) {#isFontAvailable-string-}

Indicate whether the font is available.

```javascript
static isFontAvailable(fontName: string) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontName | string | font name |

**Returns**

true if font is available, otherwise false.

### setFontSubstitutes(string, string[]) {#setFontSubstitutes-string-stringarray-}

Font substitute names for given original font name.

```javascript
static setFontSubstitutes(originalFontName: string, substituteFontNames: string[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | string | Original font name. |
| substituteFontNames | string[] | List of font substitute names to be used if original font is not presented. |

### getFontSubstitutes(string) {#getFontSubstitutes-string-}

Returns array containing font substitute names to be used if original font is not presented.

```javascript
static getFontSubstitutes(originalFontName: string) : string[];
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
static setFontFolder(fontFolder: string, recursive: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolder | string | The folder that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |

### setFontFolders(string[], boolean) {#setFontFolders-stringarray-boolean-}

Sets the fonts folders

```javascript
static setFontFolders(fontFolders: string[], recursive: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolders | string[] | The folders that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |

### setFontSources(FontSourceBase[]) {#setFontSources-fontsourcebasearray-}

Sets the fonts sources.

```javascript
static setFontSources(sources: FontSourceBase[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sources | [FontSourceBase](../fontsourcebase/)[] | An array of sources that contain TrueType fonts. |

### getFontSources() {#getFontSources--}

Gets a copy of the array that contains the list of sources

```javascript
static getFontSources() : FontSourceBase[];
```


**Returns**

[FontSourceBase](../fontsourcebase/)[]


