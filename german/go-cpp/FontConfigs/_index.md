---
title: "FontConfigs Klasse"
linktitle: "FontConfigs"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "FontConfigs Klasse. Kapselt das Objekt, das fontconfigs in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/fontconfigs/
---

## FontConfigs class

Gibt Schriftarteinstellungen an.

```go

type FontConfigs struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewFontConfigs](./newfontconfigs/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [FontConfigs_IsFontAvailable](./fontconfigs_isfontavailable/) | Gibt an, ob die Schriftart verfügbar ist. |
| [FontConfigs_GetFontFileDataInfo](./fontconfigs_getfontfiledatainfo/) | Ruft Dateninformationen der Schriftdatei ab. |
| [FontConfigs_GetDefaultFontName](./fontconfigs_getdefaultfontname/) | Liest oder setzt den Standard‑Schriftartnamen. |
| [FontConfigs_SetDefaultFontName](./fontconfigs_setdefaultfontname/) | Liest oder setzt den Standard‑Schriftartnamen. |
| [FontConfigs_GetPreferSystemFontSubstitutes](./fontconfigs_getprefersystemfontsubstitutes/) | Gibt an, ob System‑Schriftart‑Ersatz zuerst verwendet werden soll, wenn eine Schriftart nicht vorhanden ist und der Ersatz für diese Schriftart nicht festgelegt ist. z.B. Unter Ubuntu wird die Schriftart "Arial" in der Regel durch "Liberation Sans" ersetzt. Standardwert ist false. |
| [FontConfigs_SetPreferSystemFontSubstitutes](./fontconfigs_setprefersystemfontsubstitutes/) | Gibt an, ob System‑Schriftart‑Ersatz zuerst verwendet werden soll, wenn eine Schriftart nicht vorhanden ist und der Ersatz für diese Schriftart nicht festgelegt ist. z.B. Unter Ubuntu wird die Schriftart "Arial" in der Regel durch "Liberation Sans" ersetzt. Standardwert ist false. |
| [FontConfigs_SetFontSubstitutes](./fontconfigs_setfontsubstitutes/) | Schriftart‑Ersatznamen für den angegebenen ursprünglichen Schriftartnamen. |
| [FontConfigs_GetFontSubstitutes](./fontconfigs_getfontsubstitutes/) | Gibt ein Array zurück, das Schriftart‑Ersatznamen enthält, die verwendet werden, wenn die Originalschriftart nicht vorhanden ist. |
| [FontConfigs_SetFontFolder](./fontconfigs_setfontfolder/) | Legt den Schriftartenordner fest |
| [FontConfigs_SetFontFolders](./fontconfigs_setfontfolders/) | Legt den Schriftartenordner fest |
| [FontConfigs_SetFontSources](./fontconfigs_setfontsources/) | Legt die Schriftartquellen fest. |
| [FontConfigs_GetFontSources](./fontconfigs_getfontsources/) | Erhält eine Kopie des Arrays, das die Liste der Quellen enthält |
