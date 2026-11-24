---
title: "ListObject.TableStyleType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Eigenschaft. Gibt den integrierten Tabellenvorlagenstil zurück"
type: docs
url: /de/net/aspose.cells.tables/listobject/tablestyletype/
---
## ListObject.TableStyleType property

Ermittelt und die integrierte Tabellenformatvorlage.

```csharp
public TableStyleType TableStyleType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i+1}-{j+1}");
                }
            }
            
            // ListObject-Sammlung abrufen
            ListObjectCollection tables = worksheet.ListObjects;
            
            // Eine Tabelle hinzufügen
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[0];
            
            // Tabellenstil festlegen
            table.TableStyleType = TableStyleType.TableStyleDark2;
            
            // Speichere die Arbeitsmappe
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TableStyleType](../../tablestyletype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


