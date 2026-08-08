---
title: "FontConfigs"
linktitle: "FontConfigs"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Specifies font settings"
type: docs
weight: 1540
url: /nodejs/aspose.cells/fontconfigs/
---

## FontConfigs class

Specifies font settings

```js
new FontConfigs()
```

## Methods

| Name | Description |
| --- | --- |
| [getDefaultFontName()](#getdefaultfontname) | Gets or sets the default font name. |
| [setDefaultFontName()](#setdefaultfontname) | Gets or sets the default font name. |
| [getFontFileDataInfo()](#getfontfiledatainfo) *(static)* |  |
| [getFontSources()](#getfontsources) *(static)* | Gets a copy of the array that contains the list of sources |
| [getFontSubstitutes(originalFontName)](#getfontsubstitutes) *(static)* | Returns array containing font substitute names to be used if original font is not presented. |
| [isFontAvailable(fontName)](#isfontavailable) *(static)* | Indicate whether the font is available. |
| [setFontExclusiveSources(exclusiveSources)](#setfontexclusivesources) *(static)* | Sets the fonts exclusive sources. Only fonts in the sources will be used. System.setProperty("Aspose.Cells.FontDirExc",  |
| [setFontFolder(fontFolder, recursive)](#setfontfolder) *(static)* | Sets the fonts folder |
| [setFontFolders(fontFolders, recursive)](#setfontfolders) *(static)* | Sets the fonts folders |
| [setFontSources(sources)](#setfontsources) *(static)* | Sets the fonts sources. |
| [setFontSubstitutes(originalFontName, substituteFontNames)](#setfontsubstitutes) *(static)* | Font substitute names for given original font name. |

### getDefaultFontName() {#getdefaultfontname}

Gets or sets the default font name.

### setDefaultFontName() {#setdefaultfontname}

Gets or sets the default font name.

### getFontFileDataInfo() (static) {#getfontfiledatainfo}

### getFontSources() (static) {#getfontsources}

Gets a copy of the array that contains the list of sources

**Returns:** Array ofFontSourceBase — `Array ofFontSourceBase`

### getFontSubstitutes(originalFontName) (static) {#getfontsubstitutes}

Returns array containing font substitute names to be used if original font is not presented.

| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | String | originalFontName |

**Returns:** Array of String — `Array of String` An array containing font substitute names to be used if original font is not presented.

### isFontAvailable(fontName) (static) {#isfontavailable}

Indicate whether the font is available.

| Parameter | Type | Description |
| --- | --- | --- |
| fontName | String | font name |

**Returns:** boolean — `boolean` true if font is available, otherwise false.

### setFontExclusiveSources(exclusiveSources) (static) {#setfontexclusivesources}

Sets the fonts exclusive sources. Only fonts in the sources will be used. System.setProperty("Aspose.Cells.FontDirExc", "fontExclusiveFolder") will be ignored if this is set.

| Parameter | Type | Description |
| --- | --- | --- |
| exclusiveSources | Array ofFontSourceBase | An array of sources that contain TrueType fonts. |

### setFontFolder(fontFolder, recursive) (static) {#setfontfolder}

Sets the fonts folder

| Parameter | Type | Description |
| --- | --- | --- |
| fontFolder | String | The folder that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |

### setFontFolders(fontFolders, recursive) (static) {#setfontfolders}

Sets the fonts folders

| Parameter | Type | Description |
| --- | --- | --- |
| fontFolders | Array of String | The folders that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |

### setFontSources(sources) (static) {#setfontsources}

Sets the fonts sources.

| Parameter | Type | Description |
| --- | --- | --- |
| sources | Array ofFontSourceBase | An array of sources that contain TrueType fonts. |

### setFontSubstitutes(originalFontName, substituteFontNames) (static) {#setfontsubstitutes}

Font substitute names for given original font name.

| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | String | Original font name. |
| substituteFontNames | Array of String | List of font substitute names to be used if original font is not presented. |
