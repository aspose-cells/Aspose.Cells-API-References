---
title: "Workbook.GetStyleInPool"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Gibt den Stil im Stil-Pool zurück. Alle Stile im Arbeitsbuch werden in einen Pool gesammelt. In den Zellen gibt es nur einen einfachen Referenzindex."
type: docs
url: /de/net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

Ermittelt den Stil im Stil‑Pool. Alle Stile in der Arbeitsmappe werden in einen Pool gesammelt. In den Zellen gibt es nur einen einfachen Referenz‑Index.

```csharp
public Style GetStyleInPool(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index. |

### Rückgabewert

Der Stil im Pool entspricht dem angegebenen Index, kann null sein.

### Hinweise

Wenn der zurückgegebene Stil geändert wird, ändert sich der Stil aller Zellen (die auf diesen Stil verweisen).

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetStyleInPoolWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt zu und fügen Sie Beispieldaten hinzu.
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123.45);
            ws.Cells["A3"].PutValue(DateTime.Now);
            
            // Einige Stile anwenden
            Style style1 = wb.CreateStyle();
            style1.Custom = "$#,##0.00";
            ws.Cells["A2"].SetStyle(style1);
            
            Style style2 = wb.CreateStyle();
            style2.Custom = "yyyy-mm-dd";
            ws.Cells["A3"].SetStyle(style2);
            
            // In den Speicherstream speichern
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                
                // Arbeitsmappe aus Stream neu laden
                ms.Position = 0;
                Workbook reloadWb = new Workbook(ms);
                
                // Stile aus dem Stilpool abrufen und anzeigen
                int count = reloadWb.CountOfStylesInPool;
                Console.WriteLine($"Styles in pool: {count}");
                
                for (int i = 0; i < count; i++)
                {
                    Style style = reloadWb.GetStyleInPool(i);
                    Console.WriteLine($"Style {i}: CustomFormat={style.Custom}");
                }
            }
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


