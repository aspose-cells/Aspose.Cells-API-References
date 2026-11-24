---
title: "Workbook.GetNamedStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Gibt den benannten Stil im Stil-Pool zurück"
type: docs
url: /de/net/aspose.cells/workbook/getnamedstyle/
---
## Workbook.GetNamedStyle method

Ermittelt den benannten Stil im Stil‑Pool.

```csharp
public Style GetNamedStyle(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Name des Stils |

### Rückgabewert

Benannter Stil, möglicherweise null.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetNamedStyleWithStringDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Einige benannte Stile hinzufügen
            Style style1 = workbook.CreateStyle();
            style1.Name = "Number7";
            style1.Custom = "#,##0.00";
            
            Style style2 = workbook.CreateStyle();
            style2.Name = "Center";
            style2.HorizontalAlignment = TextAlignmentType.Center;
            
            // Erstelle Beispieldaten
            DataTable dt = new DataTable();
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("ProductName", typeof(string));
            dt.Columns.Add("Quantity", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            dt.Columns.Add("Discount", typeof(float));
            
            dt.Rows.Add(1, "Product A", 10, 19.99m, 0.1f);
            dt.Rows.Add(2, "Product B", 5, 29.99m, 0.15f);
            
            // Arbeitsblatt und Zellen abrufen
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Benannte Stile abrufen
            Style numberStyle = workbook.GetNamedStyle("Number7");
            Style centerStyle = workbook.GetNamedStyle("Center");
            
            // Stile auf Daten anwenden
            for(int i = 0; i < dt.Rows.Count; i++)
            {
                cells[i, 0].PutValue((int)dt.Rows[i]["ProductID"]);
                cells[i, 0].SetStyle(centerStyle);
                
                cells[i, 1].PutValue((string)dt.Rows[i]["ProductName"]);
                
                cells[i, 3].PutValue((decimal)dt.Rows[i]["UnitPrice"]);
                cells[i, 3].SetStyle(numberStyle);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("GetNamedStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


