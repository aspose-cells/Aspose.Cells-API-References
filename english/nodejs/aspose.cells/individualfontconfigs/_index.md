---
title: "IndividualFontConfigs"
linktitle: "IndividualFontConfigs"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Font configs for each Workbook object."
type: docs
weight: 1920
url: /nodejs/aspose.cells/individualfontconfigs/
---

## IndividualFontConfigs class

Font configs for each Workbook object.

```js
new IndividualFontConfigs()
```

Ctor.

## Methods

| Name | Description |
| --- | --- |
| [getFontSources()](#getfontsources) | Gets a copy of the array that contains the list of sources |
| [getFontSubstitutes(originalFontName)](#getfontsubstitutes) | Returns array containing font substitute names to be used if original font is not presented. |
| [setFontExclusiveSources(exclusiveSources)](#setfontexclusivesources) | Sets the fonts exclusive sources. Only fonts in the sources will be used. System.setProperty("Aspose.Cells.FontDirExc",  |
| [setFontFolder(fontFolder, recursive)](#setfontfolder) | Sets the fonts folder |
| [setFontFolders(fontFolders, recursive)](#setfontfolders) | Sets the fonts folders |
| [setFontSources(sources)](#setfontsources) | Sets the fonts sources. |
| [setFontSubstitutes(originalFontName, substituteFontNames)](#setfontsubstitutes) | Font substitute names for given original font name. |

### getFontSources() {#getfontsources}

Gets a copy of the array that contains the list of sources

**Returns:** Array ofFontSourceBase — `Array ofFontSourceBase`

### getFontSubstitutes(originalFontName) {#getfontsubstitutes}

Returns array containing font substitute names to be used if original font is not presented.

| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | String | originalFontName |

**Returns:** Array of String — `Array of String` An array containing font substitute names to be used if original font is not presented.

### setFontExclusiveSources(exclusiveSources) {#setfontexclusivesources}

Sets the fonts exclusive sources. Only fonts in the sources will be used. System.setProperty("Aspose.Cells.FontDirExc", "fontExclusiveFolder") will be ignored if this is set.

| Parameter | Type | Description |
| --- | --- | --- |
| exclusiveSources | Array ofFontSourceBase | An array of sources that contain TrueType fonts. |

### setFontFolder(fontFolder, recursive) {#setfontfolder}

Sets the fonts folder

| Parameter | Type | Description |
| --- | --- | --- |
| fontFolder | String | The folder that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |

### setFontFolders(fontFolders, recursive) {#setfontfolders}

Sets the fonts folders

| Parameter | Type | Description |
| --- | --- | --- |
| fontFolders | Array of String | The folders that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |

### setFontSources(sources) {#setfontsources}

Sets the fonts sources.

| Parameter | Type | Description |
| --- | --- | --- |
| sources | Array ofFontSourceBase | An array of sources that contain TrueType fonts. |

### setFontSubstitutes(originalFontName, substituteFontNames) {#setfontsubstitutes}

Font substitute names for given original font name.

| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | String | Original font name. |
| substituteFontNames | Array of String | List of font substitute names to be used if original font is not presented. |
