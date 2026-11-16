---
title: "LowCodeSaveOptionsProviderOfPlaceHolders-Klasse"
linktitle: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "LowCodeSaveOptionsProviderOfPlaceHolders-Klasse. Kapselt das Objekt, das lowcodesaveoptionsproviderofplaceholders in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/lowcodesaveoptionsproviderofplaceholders/
---

## LowCodeSaveOptionsProviderOfPlaceHolders class

Implementierung zur Bereitstellung von Speicheroptionen, die geteilte Teile in Dateien speichern und deren Pfad mit Platzhaltern definiert ist.

```go

type LowCodeSaveOptionsProviderOfPlaceHolders struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_String](./newlowcodesaveoptionsproviderofplaceholders_string/) | Instanziiert eine Instanz, um Speicheroptionen gemäß den angegebenen Vorlagen bereitzustellen. |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofplaceholders_abstractlowcodesaveoptionsprovider/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | Versatz des Blattindexes zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert (SplitPartInfo.SheetIndex). |
| [SetSheetIndexOffset](./setsheetindexoffset/) | Versatz des Blattindexes zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert (SplitPartInfo.SheetIndex). |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | Versatz des Indexes des geteilten Teils zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert (SplitPartInfo.PartIndex). |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | Versatz des Indexes des geteilten Teils zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert (SplitPartInfo.PartIndex). |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | Ob der Blattindex oder -name immer zum Dateipfad hinzugefügt wird. Der Standardwert ist false, das heißt, wenn nur ein Blatt vorhanden ist, werden der Blattindex und -name sowie das entsprechende Präfix (SheetNamePrefix) nicht zum Dateipfad hinzugefügt. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | Ob der Blattindex oder -name immer zum Dateipfad hinzugefügt wird. Der Standardwert ist false, das heißt, wenn nur ein Blatt vorhanden ist, werden der Blattindex und -name sowie das entsprechende Präfix (SheetNamePrefix) nicht zum Dateipfad hinzugefügt. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | Ob der Index des geteilten Teils immer zum Dateipfad hinzugefügt wird. Standardwert ist false, das heißt, wenn es nur einen geteilten Teil gibt, werden der Index des geteilten Teils und das entsprechende Präfix (SplitPartPrefix) nicht zum Dateipfad hinzugefügt. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | Ob der Index des geteilten Teils immer zum Dateipfad hinzugefügt wird. Standardwert ist false, das heißt, wenn es nur einen geteilten Teil gibt, werden der Index des geteilten Teils und das entsprechende Präfix (SplitPartPrefix) nicht zum Dateipfad hinzugefügt. |
| [GetSheetNamePrefix](./getsheetnameprefix/) | Präfix für den Index des Arbeitsblatts. |
| [SetSheetNamePrefix](./setsheetnameprefix/) | Präfix für den Index des Arbeitsblatts. |
| [GetSheetIndexPrefix](./getsheetindexprefix/) | Präfix für den Index des Arbeitsblatts. |
| [SetSheetIndexPrefix](./setsheetindexprefix/) | Präfix für den Index des Arbeitsblatts. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | Präfix für den Index des geteilten Teils. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | Präfix für den Index des geteilten Teils. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | Die Vorlage zum Erstellen einer Instanz von Speicheroptionen in GetSaveOptions(SplitPartInfo). |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | Die Vorlage zum Erstellen einer Instanz von Speicheroptionen in GetSaveOptions(SplitPartInfo). |
| [GetSaveOptions](./getsaveoptions/) | Ruft die Speicheroptionen ab, aus denen die Ausgabeeinstellungen für das aktuell geteilte Teil erhalten werden. |
| [Finish](./finish/) | Gibt Ressourcen nach der Verarbeitung des aktuell geteilten Teils frei. |
