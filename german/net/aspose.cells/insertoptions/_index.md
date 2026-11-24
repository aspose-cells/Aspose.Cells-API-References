---
title: "Klasse InsertOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.InsertOptions Klasse. Stellt die Optionen für das Einfügen dar."
type: docs
url: /de/net/aspose.cells/insertoptions/
---
## InsertOptions class

Stellt die Optionen für das Einfügen dar.

```csharp
public class InsertOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [InsertOptions](insertoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CopyFormatType](../../aspose.cells/insertoptions/copyformattype/) { get; set; } |  |
| [FormulaChangeMonitor](../../aspose.cells/insertoptions/formulachangemonitor/) { get; set; } | Liest/setzt den Monitor zur Verfolgung von Änderungen, die durch das Einfügen verursacht werden. |
| [UpdateReference](../../aspose.cells/insertoptions/updatereference/) { get; set; } | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsDemo
    {
        public static void InsertOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz von InsertOptions
            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Definiere den Zellbereich, in dem Zeilen eingefügt werden sollen
            CellArea cellArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };

            // Füge Zeilen mit den angegebenen Optionen ein
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("InsertOptionsExample.xlsx");
            workbook.Save("InsertOptionsExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


