---
title: "ListObject.UpdateColumnName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject‑Methode. Aktualisiert alle ListColumn‑Namen in die Zellen der Tabelle"
type: docs
url: /de/net/aspose.cells.tables/listobject/updatecolumnname/
---
## ListObject.UpdateColumnName method

Aktualisiert alle Namen der Listenspalten in den Zellen der Tabelle.

```csharp
public void UpdateColumnName()
```

### Hinweise

Der Wert der Zellen in der Kopfzeile der Tabelle muss dem Namen der ListColumn entsprechen; Cell.PutValue ändert den Namen der ListColumn aus Leistungsgründen nicht automatisch.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectMethodUpdateColumnNameDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Ein Tabellen-/Listenobjekt erstellen
            var listObject = ws.ListObjects[ws.ListObjects.Add(3, 3, 6, 6, true)];
            
            // Einige Daten in der Tabelle befüllen
            for (int r = 0; r < 3; r++)
            {
                for (int c = 0; c < 3; c++)
                {
                    if (c > 0)
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue(r + c);
                    else
                        ws.Cells[listObject.StartRow + r, listObject.StartColumn + c].PutValue("");
                }
            }

            // Spaltennamen aktualisieren (setzt Standardnamen wie Column1, Column2 usw.)
            listObject.UpdateColumnName();

            // Speichere die Arbeitsmappe
            wb.Save("output.xlsx");

            // Überprüfen, ob der Spaltenname aktualisiert wurde
            Console.WriteLine("First column name: " + ws.Cells[listObject.StartRow, listObject.StartColumn].StringValue);
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


