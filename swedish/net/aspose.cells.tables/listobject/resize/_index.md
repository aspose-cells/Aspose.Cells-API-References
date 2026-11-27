---
title: "ListObject.Resize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListObject-metod. Ändra storlek på området för listobjektet"
type: docs
url: /sv/net/aspose.cells.tables/listobject/resize/
---
## ListObject.Resize method

Ändra storlek på intervallet för listobjektet.

```csharp
public void Resize(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startradens index för det nya området. |
| startColumn | Int32 | Startkolumnens index för det nya området. |
| endRow | Int32 | Slutradens index för det nya området. |
| endColumn | Int32 | Slutkolumnens index för det nya området. |
| hasHeaders | Boolean | Om den här tabellen har rubriker. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodResizeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue("Item " + (i + 1));
                worksheet.Cells[i, 1].PutValue(i * 10);
            }

            // Skapa ett listobjekt
            int index = worksheet.ListObjects.Add(0, 0, 5, 1, true);
            ListObject listObj = worksheet.ListObjects[index];
            listObj.TableStyleType = TableStyleType.TableStyleLight2;

            // Ändra storlek på listobjektet
            listObj.Resize(0, 0, 9, 1, true);

            // Spara arbetsboken
            workbook.Save("ResizedListObject.xlsx");
        }
    }
}
```

### Se även

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


