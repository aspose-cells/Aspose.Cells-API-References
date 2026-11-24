---
title: "TxtSaveOptions.ExportArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Eigenschaft. Der Bereich der zu exportierenden Zellen"
type: docs
url: /de/net/aspose.cells/txtsaveoptions/exportarea/
---
## TxtSaveOptions.ExportArea property

Der zu exportierende Zellbereich.

```csharp
public CellArea ExportArea { get; set; }
```

### Hinweise

Wenn der Exportbereich angegeben wurde, hat [`TrimLeadingBlankRowAndColumn`](../trimleadingblankrowandcolumn/) keine Wirkung.

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zellen mit Daten füllen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(699.99);
            worksheet.Cells["A4"].PutValue("Tablet");
            worksheet.Cells["B4"].PutValue(399.99);

            // Text‑Speicheroptionen mit ExportArea konfigurieren
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = '\t',
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // Nur den angegebenen Bereich speichern (erste 3 Zeilen, erste 2 Spalten)
            workbook.Save("ExportedData.txt", saveOptions);

            Console.WriteLine("Data exported successfully with ExportArea restriction.");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


