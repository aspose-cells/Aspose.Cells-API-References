---
title: "TxtSaveOptions.TrimTailingBlankCells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Eigenschaft. Gibt an, ob nachfolgende leere Zellen in einer Zeile abgeschnitten werden sollen. Standard ist false."
type: docs
url: /de/net/aspose.cells/txtsaveoptions/trimtailingblankcells/
---
## TxtSaveOptions.TrimTailingBlankCells property

Gibt an, ob nachfolgende leere Zellen in einer Zeile entfernt werden sollen. Standard ist false.

```csharp
public bool TrimTailingBlankCells { get; set; }
```

### Hinweise

Beim Speichern im LightCells‑Modus und wenn das [`ExportArea`](../exportarea/) nicht angegeben wurde, hat diese Option keine Wirkung und eine Zeile wird bis zur letzten von der Implementierung [`LightCellsDataProvider`](../lightcellsdataprovider/) bereitgestellten Zelle erweitert.

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimTailingBlankCellsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Fügen Sie Beispieldaten hinzu
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[0, 2].PutValue("C");
            cells[1, 0].PutValue(1);
            cells[1, 2].PutValue(2);
            cells[2, 0].PutValue(3);

            // Speichern ohne Abschneiden nachfolgender leerer Zellen (Standard)
            TxtSaveOptions options1 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = false
            };
            string result1 = SaveAsCsv(workbook, options1);
            Console.WriteLine("Without TrimTailingBlankCells:\n" + result1);

            // Speichern mit Abschneiden nachfolgender leerer Zellen
            TxtSaveOptions options2 = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                TrimTailingBlankCells = true
            };
            string result2 = SaveAsCsv(workbook, options2);
            Console.WriteLine("\nWith TrimTailingBlankCells:\n" + result2);
        }

        private static string SaveAsCsv(Workbook workbook, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                workbook.Save(stream, options);
                return Encoding.ASCII.GetString(stream.ToArray());
            }
        }
    }
}
```

### Siehe auch

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


