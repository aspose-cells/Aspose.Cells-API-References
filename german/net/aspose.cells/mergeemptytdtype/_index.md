---
title: "Aufzählung MergeEmptyTdType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.MergeEmptyTdType Aufzählung. Stellt den Zusammenführungs‑Typ für ein leeres TD‑Element beim Export einer Datei nach HTML dar"
type: docs
url: /de/net/aspose.cells/mergeemptytdtype/
---
## MergeEmptyTdType enumeration

Stellt den Zusammenführungs-Typ für ein leeres TD-Element beim Exportieren einer Datei nach HTML dar.

```csharp
public enum MergeEmptyTdType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Default | `0` | Anzeige wie in MS Excel. |
| None | `1` | Leere TD‑Elemente werden beim Export einer Datei nach HTML nicht zusammengeführt. Dies erzeugt eine deutlich größere HTML‑Datei. |
| MergeForcely | `2` | Leere TD‑Elemente werden beim Export einer Datei nach HTML zwangsweise zusammengeführt. Die Größe der HTML‑Datei wird nach dem Setzen des Wertes auf true deutlich reduziert. Wenn Sie die HTML‑Datei nach Excel importieren oder beim Speichern der Datei nach HTML perfekte Gitternetzlinien exportieren möchten, behalten Sie bitte den Standardwert bei. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MergeEmptyTdTypeDemo
    {
        public static void MergeEmptyTdTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Data1");
            worksheet.Cells["B1"].PutValue("Data2");
            worksheet.Cells["C1"].PutValue("Data3");

            // Erstellen Sie HtmlSaveOptions und setzen Sie die MergeEmptyTdType‑Eigenschaft
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.MergeForcely;

            // Speichere das Arbeitsbuch im HTML‑Format
            workbook.Save("MergeEmptyTdTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with MergeEmptyTdType.MergeForcely option.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


