---
title: "ListObject.ListColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Eigenschaft. Gibt die ListColumn-Liste dieser Tabelle zurück"
type: docs
url: /de/net/aspose.cells.tables/listobject/listcolumns/
---
## ListObject.ListColumns property

Ruft die [`ListColumn`](../../listcolumn/) Liste dieser Tabelle ab.

```csharp
public ListColumnCollection ListColumns { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyListColumnsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Erstelle ein Listenobjekt
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add(0, 0, 9, 4, true);
            ListObject listObject = listObjects[index];
            
            // Summen aktivieren und Berechnung für die 5. Spalte festlegen
            listObject.ShowTotals = true;
            listObject.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
            
            // Tabellenstil anwenden
            listObject.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleLight4;

            // Speichere die Arbeitsmappe
            workbook.Save("ListColumnsDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListColumnCollection](../../listcolumncollection/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


