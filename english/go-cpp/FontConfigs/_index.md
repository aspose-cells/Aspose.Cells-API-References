---
title: FontConfigs Class 
linktitle: FontConfigs
second_title: Aspose.Cells for Go via C++ API Reference
description: 'FontConfigs class. Encapsulates the object that represents fontconfigs in Go.'
type: docs
weight: 200
url: /go-cpp/fontconfigs/
---

## FontConfigs class

Specifies font settings

```go

type FontConfigs struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewFontConfigs](./newfontconfigs/) | Default constructor. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[FontConfigs_IsFontAvailable](./fontconfigs_isfontavailable/) | Indicate whether the font is available. | 
|[FontConfigs_GetFontFileDataInfo](./fontconfigs_getfontfiledatainfo/) | Get data information of font file data. | 
|[FontConfigs_GetDefaultFontName](./fontconfigs_getdefaultfontname/) | Gets or sets the default font name. | 
|[FontConfigs_SetDefaultFontName](./fontconfigs_setdefaultfontname/) | Gets or sets the default font name. | 
|[FontConfigs_GetPreferSystemFontSubstitutes](./fontconfigs_getprefersystemfontsubstitutes/) | Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set.e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans".Default value is false. | 
|[FontConfigs_SetPreferSystemFontSubstitutes](./fontconfigs_setprefersystemfontsubstitutes/) | Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set.e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans".Default value is false. | 
|[FontConfigs_SetFontSubstitutes](./fontconfigs_setfontsubstitutes/) | Font substitute names for given original font name. | 
|[FontConfigs_GetFontSubstitutes](./fontconfigs_getfontsubstitutes/) | Returns an array containing font substitute names to be used if original font is not present. | 
|[FontConfigs_SetFontFolder](./fontconfigs_setfontfolder/) | Sets the fonts folder | 
|[FontConfigs_SetFontFolders](./fontconfigs_setfontfolders/) | Sets the fonts folder | 
|[FontConfigs_SetFontSources](./fontconfigs_setfontsources/) | Sets the font sources. | 
|[FontConfigs_GetFontSources](./fontconfigs_getfontsources/) | Gets a copy of the array that contains the list of sources | 
