---
title: "TxtSaveOptions.KeepSeparatorsForBlankRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Eigenschaft. Gibt an, ob Trennzeichen für leere Zeilen ausgegeben werden sollen. Der Standardwert ist false, sodass der Inhalt für leere Zeilen standardmäßig leer ist."
type: docs
url: /de/net/aspose.cells/txtsaveoptions/keepseparatorsforblankrow/
---
## TxtSaveOptions.KeepSeparatorsForBlankRow property

Gibt an, ob Trennzeichen für leere Zeilen ausgegeben werden sollen. Der Standardwert ist false, sodass der Inhalt einer leeren Zeile standardmäßig leer ist.

```csharp
public bool KeepSeparatorsForBlankRow { get; set; }
```

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyKeepSeparatorsForBlankRowDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Fügen Sie einige Daten mit leeren Zeilen hinzu
            cells[0, 0].PutValue("a");
            cells[0, 1].PutValue("b");
            cells[3, 0].PutValue("c");
            cells[4, 1].PutValue("d");

            // Speicheroptionen erstellen mit KeepSeparatorsForBlankRow auf true gesetzt
            TxtSaveOptions options = new TxtSaveOptions
            {
                Encoding = Encoding.ASCII,
                KeepSeparatorsForBlankRow = true
            };

            // Arbeitsmappe mit den Optionen als CSV speichern
            string csvOutput = SaveAsCsv(wb, options);
            Console.WriteLine(csvOutput);
        }

        private static string SaveAsCsv(Workbook wb, TxtSaveOptions options)
        {
            using (System.IO.MemoryStream stream = new System.IO.MemoryStream())
            {
                wb.Save(stream, options);
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


