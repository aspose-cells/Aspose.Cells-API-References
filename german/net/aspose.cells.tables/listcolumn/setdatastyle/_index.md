---
title: "ListColumn.SetDataStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListColumn-Methode. Legt den Stil der Daten in dieser Spalte der Tabelle fest."
type: docs
url: /de/net/aspose.cells.tables/listcolumn/setdatastyle/
---
## ListColumn.SetDataStyle method

Setzt den Stil der Daten in dieser Spalte der Tabelle.

```csharp
public void SetDataStyle(Style style)
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListColumnMethodSetDataStyleWithStyleDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Erstelle ein Listenobjekt (Tabelle)
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
            
            // Erhalte den Stil der ersten Spalte.
            Style style = table.ListColumns[0].GetDataStyle();
            
            // Stil ändern
            style.Pattern = BackgroundType.Solid;
            style.BackgroundColor = System.Drawing.Color.Red;
            
            // Wende den modifizierten Stil auf die Spalte an.
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


