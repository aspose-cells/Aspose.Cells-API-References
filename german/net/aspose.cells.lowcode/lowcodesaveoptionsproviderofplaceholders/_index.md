---
title: "Klasse LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfPlaceHolders Klasse. Implementierung zur Bereitstellung von Speicheroptionen, die geteilte Teile in Dateien speichern, wobei der Pfad der resultierenden Datei mit Platzhaltern definiert wird."
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/
---
## LowCodeSaveOptionsProviderOfPlaceHolders class

Implementierung zur Bereitstellung von Speicheroptionen, die geteilte Teile in Dateien speichern und der Pfad der resultierenden Datei mit Platzhaltern definiert wird.

```csharp
public class LowCodeSaveOptionsProviderOfPlaceHolders : AbstractLowCodeSaveOptionsProvider
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders](lowcodesaveoptionsproviderofplaceholders/)(string) | Instanziiert eine Instanz, um Speicheroptionen gemäß den angegebenen Vorlagen bereitzustellen. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/) { get; set; } | Ob der Blattindex oder -name immer zum Dateipfad hinzugefügt wird. Der Standardwert ist false, das heißt, wenn nur ein Blatt vorhanden ist, werden der Blattindex und -name sowie das entsprechende Präfix([`SheetNamePrefix`](./sheetnameprefix/)) nicht zum Dateipfad hinzugefügt. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/) { get; set; } | Ob der Index des geteilten Teils immer zum Dateipfad hinzugefügt wird. Der Standardwert ist false, das heißt, wenn nur ein geteiltes Teil vorhanden ist, werden der Index des geteilten Teils und das entsprechende Präfix([`SplitPartPrefix`](./splitpartprefix/)) nicht zum Dateipfad hinzugefügt. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/) { get; set; } | Die Vorlage zur Erstellung einer Instanz von Speicheroptionen in [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/) { get; set; } | Versatz des Blatt‑Index zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert ([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetIndexPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/) { get; set; } | Präfix für den Index des Arbeitsblatts. |
| [SheetNamePrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/) { get; set; } | Präfix für den Index des Arbeitsblatts. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/) { get; set; } | Versatz des Index des geteilten Teils zwischen dem im Dateipfad verwendeten Wert und seinem tatsächlichen Wert ([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/) { get; set; } | Präfix für den Index des geteilten Teils. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Gibt Ressourcen nach der Verarbeitung des aktuellen geteilten Teils frei. (Vererbt von [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/)(SplitPartInfo) | Liest die Speicheroptionen, aus denen die Ausgabeeinstellungen für das aktuelle geteilte Teil abgerufen werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;

    public class LowCodeClassLowCodeSaveOptionsProviderOfPlaceHoldersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Arbeitsblatt mit Beispieldaten füllen
            for (int i = 0; i < 250; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // Erstellen Sie einen Provider mit Pfadvorlage, die Platzhalter enthält.
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_Sheet_{sheet}_Part_{split}.xlsx");
            
            // Konfigurieren Sie die Provider-Eigenschaften.
            provider.SheetIndexOffset = 1;
            provider.SplitPartIndexOffset = 1;
            provider.SheetIndexPrefix = "S";
            provider.SplitPartPrefix = "P";
            provider.BuildPathWithSheetAlways = true;
            provider.BuildPathWithSplitPartAlways = true;

            // Konfigurieren Sie die Vorlage für Speicheroptionen.
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx
            };

            // Konfigurieren Sie Bild- oder Druckoptionen für die geteilte Darstellung.
            var imgOrPrintOptions = new ImageOrPrintOptions
            {
                SaveFormat = SaveFormat.Pdf,
                OnePagePerSheet = false,
                PageIndex = 0,
                PageCount = 1
            };

            // Erstellen Sie die Blattdarstellung mit geteilter Konfiguration.
            var sheetRender = new SheetRender(worksheet, imgOrPrintOptions);
            sheetRender.ToImage(0, "output"); // This would normally split and save using provider
        }
    }
}
```

### Siehe auch

* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


