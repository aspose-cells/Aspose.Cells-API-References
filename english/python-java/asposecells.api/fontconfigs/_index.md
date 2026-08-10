---
title: "FontConfigs Class"
linktitle: "FontConfigs"
articleTitle: "FontConfigs"
second_title: "Aspose.Cells for Python via Java"
description: "Specifies font settings"
type: docs
weight: 2440
url: /python-java/asposecells.api/fontconfigs/
---

## FontConfigs class

Specifies font settings

## Constructors

| Name | Description |
| --- | --- |
| [FontConfigs](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [DefaultFontName](#defaultfontname) | String | Gets or sets the default font name. |

## Methods

| Name | Description |
| --- | --- |
| [isFontAvailable](#isfontavailable) | Indicate whether the font is available. |
| [getFontFileDataInfo](#getfontfiledatainfo) |  |
| [setFontSubstitutes](#setfontsubstitutes) | Font substitute names for given original font name. |
| [getFontSubstitutes](#getfontsubstitutes) | Returns array containing font substitute names to be used if original font is not presented. |
| [setFontFolder](#setfontfolder) | Sets the fonts folder |
| [setFontFolders](#setfontfolders) | Sets the fonts folders |
| [setFontSources](#setfontsources) | Sets the fonts sources. |
| [setFontExclusiveSources](#setfontexclusivesources) | Sets the fonts exclusive sources. Only fonts in the sources will be used.

System.setProperty("Aspose.Cells.FontDirExc", |
| [getFontSources](#getfontsources) | Gets a copy of the array that contains the list of sources |

### FontConfigs() {#constructor}

### FontConfigs.DefaultFontName property {#defaultfontname}

Gets or sets the default font name.

**Type:** String

### isFontAvailable(fontName) {#isfontavailable}

Indicate whether the font is available.

| Parameter | Type | Description |
| --- | --- | --- |
| fontName | String | font name |

**Returns:** true if font is available, otherwise false.

### getFontFileDataInfo(fontName, isBold, isItalic, isExactStyle) {#getfontfiledatainfo}

### setFontSubstitutes(originalFontName, substituteFontNames) {#setfontsubstitutes}

Font substitute names for given original font name.

| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | String | Original font name. |
| substituteFontNames | String[] | List of font substitute names to be used if original font is not presented. |

### getFontSubstitutes(originalFontName) {#getfontsubstitutes}

Returns array containing font substitute names to be used if original font is not presented.

| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | String | originalFontName |

**Returns:** An array containing font substitute names to be used if original font is not presented.

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
| fontFolders | String[] | The folders that contains TrueType fonts. |
| recursive | boolean | Determines whether or not to scan subfolders. |

### setFontSources(sources) {#setfontsources}

Sets the fonts sources.

| Parameter | Type | Description |
| --- | --- | --- |
| sources | FontSourceBase[] | An array of sources that contain TrueType fonts. |

### setFontExclusiveSources(exclusiveSources) {#setfontexclusivesources}

Sets the fonts exclusive sources. Only fonts in the sources will be used.

System.setProperty("Aspose.Cells.FontDirExc", "fontExclusiveFolder") will be ignored if this is set.

| Parameter | Type | Description |
| --- | --- | --- |
| exclusiveSources | FontSourceBase[] | An array of sources that contain TrueType fonts. |

### getFontSources() {#getfontsources}

Gets a copy of the array that contains the list of sources
