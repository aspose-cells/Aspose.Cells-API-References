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

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| static [defaultFontName](#defaultFontName--)| string | Gets or sets the default font name. |
| static [preferSystemFontSubstitutes](#preferSystemFontSubstitutes--)| boolean | Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false. |

## Methods

| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| static [getDefaultFontName()](#getDefaultFontName--)| <b>@deprecated.</b> Please use the 'defaultFontName' property instead. Gets or sets the default font name. |
| static [setDefaultFontName(string)](#setDefaultFontName-string-)| <b>@deprecated.</b> Please use the 'defaultFontName' property instead. Gets or sets the default font name. |
| static [getPreferSystemFontSubstitutes()](#getPreferSystemFontSubstitutes--)| <b>@deprecated.</b> Please use the 'preferSystemFontSubstitutes' property instead. Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false. |
| static [setPreferSystemFontSubstitutes(boolean)](#setPreferSystemFontSubstitutes-boolean-)| <b>@deprecated.</b> Please use the 'preferSystemFontSubstitutes' property instead. Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false. |
| static [isFontAvailable(string)](#isFontAvailable-string-)| Indicate whether the font is available. |
| static [getFontFileDataInfo(string, boolean, boolean, boolean)](#getFontFileDataInfo-string-boolean-boolean-boolean-)| Get data information of font file data. |
| static [setFontSubstitutes(string, string[])](#setFontSubstitutes-string-stringarray-)| Font substitute names for given original font name. |
| static [getFontSubstitutes(string)](#getFontSubstitutes-string-)| Returns an array containing font substitute names to be used if original font is not present. |
| static [setFontFolder(string, boolean)](#setFontFolder-string-boolean-)| Sets the fonts folder |
| static [setFontFolders(string[], boolean)](#setFontFolders-stringarray-boolean-)| Sets the fonts folder |
| static [setFontSources(FontSourceBase[])](#setFontSources-fontsourcebasearray-)| Sets the font sources. |
| static [getFontSources()](#getFontSources--)| Gets a copy of the array that contains the list of sources |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### defaultFontName {#defaultFontName--}

Gets or sets the default font name.

```javascript
static defaultFontName : string;
```


### preferSystemFontSubstitutes {#preferSystemFontSubstitutes--}

Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false.

```javascript
static preferSystemFontSubstitutes : boolean;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getDefaultFontName() {#getDefaultFontName--}

<b>@deprecated.</b> Please use the 'defaultFontName' property instead. Gets or sets the default font name.

```javascript
static getDefaultFontName() : string;
```


### setDefaultFontName(string) {#setDefaultFontName-string-}

<b>@deprecated.</b> Please use the 'defaultFontName' property instead. Gets or sets the default font name.

```javascript
static setDefaultFontName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPreferSystemFontSubstitutes() {#getPreferSystemFontSubstitutes--}

<b>@deprecated.</b> Please use the 'preferSystemFontSubstitutes' property instead. Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false.

```javascript
static getPreferSystemFontSubstitutes() : boolean;
```


### setPreferSystemFontSubstitutes(boolean) {#setPreferSystemFontSubstitutes-boolean-}

<b>@deprecated.</b> Please use the 'preferSystemFontSubstitutes' property instead. Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false.

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

### getFontFileDataInfo(string, boolean, boolean, boolean) {#getFontFileDataInfo-string-boolean-boolean-boolean-}

Get data information of font file data.

```javascript
static getFontFileDataInfo(fontName: string, isBold: boolean, isItalic: boolean, isExactStyle: boolean) : FontFileDataInfo;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontName | string | font name |
| isBold | boolean | the font style is bold or not |
| isItalic | boolean | the font style is italic or not |
| isExactStyle | boolean | whether to match the given bold/italic style exactly |

**Returns**

Data infomation of font file data.

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

Returns an array containing font substitute names to be used if original font is not present.

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

Sets the fonts folder

```javascript
static setFontFolders(fontFolders: string[], recursive: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolders | string[] | The folders that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |

### setFontSources(FontSourceBase[]) {#setFontSources-fontsourcebasearray-}

Sets the font sources.

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


