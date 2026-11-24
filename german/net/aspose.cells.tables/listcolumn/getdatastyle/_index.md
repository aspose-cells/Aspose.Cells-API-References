---
title: "ListColumn.GetDataStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListColumn-Methode. Gibt den Stil der Daten in dieser Spalte der Tabelle zurück."
type: docs
url: /de/net/aspose.cells.tables/listcolumn/getdatastyle/
---
## ListColumn.GetDataStyle method

Liefert den Stil der Daten in dieser Spalte der Tabelle.

```csharp
public Style GetDataStyle()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetDataStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Erstelle ein Listenobjekt (Tabelle)
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            
            // Stil von der ersten ListColumn abrufen.
            Style style = table.ListColumns[0].GetDataStyle();
            
            // Stil ändern
            style.Pattern = BackgroundType.Solid;
            style.BackgroundColor = System.Drawing.Color.Red;
            
            // Den modifizierten Stil wieder auf die Spalte anwenden.
            table.ListColumns[0].SetDataStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../../aspose.cells/style/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


