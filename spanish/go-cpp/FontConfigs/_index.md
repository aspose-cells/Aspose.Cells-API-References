---
title: "Clase FontConfigs"
linktitle: "FontConfigs"
second_title: "Aspose.Cells for Go via C++ API Reference"
description: "Clase FontConfigs. Encapsula el objeto que representa fontconfigs en Go."
type: docs
weight: 200
url: /es/go-cpp/fontconfigs/
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
| [NewFontConfigs](./newfontconfigs/) | Default constructor. |

## Methods

| Method | Description |
| --- | --- |
| [IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
| [FontConfigs_IsFontAvailable](./fontconfigs_isfontavailable/) | Indica si la fuente está disponible. |
| [FontConfigs_GetFontFileDataInfo](./fontconfigs_getfontfiledatainfo/) | Obtén información de datos del archivo de fuente. |
| [FontConfigs_GetDefaultFontName](./fontconfigs_getdefaultfontname/) | Obtiene o establece el nombre de fuente predeterminado. |
| [FontConfigs_SetDefaultFontName](./fontconfigs_setdefaultfontname/) | Obtiene o establece el nombre de fuente predeterminado. |
| [FontConfigs_GetPreferSystemFontSubstitutes](./fontconfigs_getprefersystemfontsubstitutes/) | Indica si se deben usar primero los sustitutos de fuentes del sistema o no cuando una fuente no está presente y el sustituto de esa fuente no está configurado. Por ejemplo, en Ubuntu, la fuente "Arial" suele ser sustituida por "Liberation Sans". El valor predeterminado es false. |
| [FontConfigs_SetPreferSystemFontSubstitutes](./fontconfigs_setprefersystemfontsubstitutes/) | Indica si se deben usar primero los sustitutos de fuentes del sistema o no cuando una fuente no está presente y el sustituto de esa fuente no está configurado. Por ejemplo, en Ubuntu, la fuente "Arial" suele ser sustituida por "Liberation Sans". El valor predeterminado es false. |
| [FontConfigs_SetFontSubstitutes](./fontconfigs_setfontsubstitutes/) | Nombres de sustitutos de fuentes para el nombre de fuente original dado. |
| [FontConfigs_GetFontSubstitutes](./fontconfigs_getfontsubstitutes/) | Devuelve una matriz que contiene los nombres de sustitutos de fuentes que se usarán si la fuente original no está presente. |
| [FontConfigs_SetFontFolder](./fontconfigs_setfontfolder/) | Sets the fonts folder |
| [FontConfigs_SetFontFolders](./fontconfigs_setfontfolders/) | Sets the fonts folder |
| [FontConfigs_SetFontSources](./fontconfigs_setfontsources/) | Sets the font sources. |
| [FontConfigs_GetFontSources](./fontconfigs_getfontsources/) | Gets a copy of the array that contains the list of sources |
