---
title: "Klasse LowCodeSaveOptionsProviderOfAssembling"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfAssembling Klasse. Implementierung zur Bereitstellung von Speicheroptionen, die geteilte Teile in Dateien speichern, wobei der Pfad der resultierenden Datei wie folgt benannt wird und Verzeichnisse enthalten kann: PathHeader SheetPrefix SheetIndex oder SheetName SplitPartPrefix SplitPartIndex PathTail"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/
---
## LowCodeSaveOptionsProviderOfAssembling class

Implementierung zur Bereitstellung von Speicheroptionen, die geteilte Teile in Dateien speichern, wobei der Pfad der resultierenden Datei wie folgt benannt wird (es können Verzeichnisse enthalten sein): [`PathHeader`](./pathheader/)+[`SheetPrefix`](./sheetprefix/)+SheetIndex(oder SheetName)+[`SplitPartPrefix`](./splitpartprefix/)+SplitPartIndex+[`PathTail`](./pathtail/).

```csharp
public class LowCodeSaveOptionsProviderOfAssembling : AbstractLowCodeSaveOptionsProvider
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling](lowcodesaveoptionsproviderofassembling/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/) { get; set; } | Ob der Blatt‑Index oder -Name immer zum Dateipfad hinzugefügt wird. Standardwert ist false, d.h., wenn nur ein Blatt vorhanden ist, werden der Blatt‑Index (oder Name) und das entsprechende Präfix nicht zum Dateipfad hinzugefügt. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/) { get; set; } | Ob der Index des geteilten Teils immer zum Dateipfad hinzugefügt wird. Standardwert ist false, d.h., wenn nur ein geteiltes Teil vorhanden ist, werden der Teil‑Index und das entsprechende Präfix nicht zum Dateipfad hinzugefügt. |
| [PathHeader](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/) { get; set; } | Kopfteil (vor dem hinzugefügten Inhalt von Blatt und geteiltem Teil) des Dateipfads. |
| [PathTail](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/) { get; set; } | Nachtrag (nach den Sequenznummern) des Dateipfads. Er sollte die Dateinamenerweiterung enthalten. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/) { get; set; } | Die Vorlage zur Erstellung einer Instanz von Speicheroptionen in [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/) { get; set; } | Versatz des Blatt‑Index zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/) { get; set; } | Präfix für den Index des Arbeitsblatts. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/) { get; set; } | Versatz des Index des geteilten Teils zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/) { get; set; } | Präfix für den Index des geteilten Teils. |
| [UseSheetName](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/) { get; set; } | Ob der Dateipfad mit dem Blattnamen anstelle des Blatt‑Index erstellt wird. Standardwert ist false. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Gibt Ressourcen nach der Verarbeitung des aktuellen geteilten Teils frei. (Vererbt von [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/)(SplitPartInfo) | Liest die Speicheroptionen, aus denen die Ausgabeeinstellungen für das aktuelle geteilte Teil abgerufen werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;

    public class LowCodeClassLowCodeSaveOptionsProviderOfAssemblingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data {i + 1}";
            }

            // Initialisieren und konfigurieren Sie den Speicheroptionen-Provider
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitOutput/",
                PathTail = "_Part.xlsx",
                UseSheetName = true,
                SheetPrefix = "SHEET-",
                SplitPartPrefix = "PART-",
                BuildPathWithSheetAlways = true,
                BuildPathWithSplitPartAlways = true,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Konfigurieren Sie XLSX-Speicheroptionen mit Aufteilung unter Verwendung von LowCodeSaveOptions
            LowCodeSaveOptions saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Speichern Sie die Arbeitsmappe mit vom Provider aktivierten Optionen unter Verwendung des korrekten Speicherformats
            workbook.Save("LowCodeSaveOptionsProviderOfAssemblingDemo_Output.xlsx", saveOptions.SaveFormat);
        }
    }
}
```

### Siehe auch

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


