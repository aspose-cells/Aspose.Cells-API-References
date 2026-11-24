---
title: "ListObject.Resize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Methode. Ändert die Größe des Bereichs des ListObject"
type: docs
url: /de/net/aspose.cells.tables/listobject/resize/
---
## ListObject.Resize method

Ändert die Größe des Bereichs des Listobjekts.

```csharp
public void Resize(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Der Startzeilenindex des neuen Bereichs. |
| startColumn | Int32 | Der Startspaltenindex des neuen Bereichs. |
| endRow | Int32 | Der Endzeilenindex des neuen Bereichs. |
| endColumn | Int32 | Der Endspaltenindex des neuen Bereichs. |
| hasHeaders | Boolean | Ob diese Tabelle Überschriften hat. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue("Item " + (i + 1));
                worksheet.Cells[i, 1].PutValue(i * 10);
            }

            // Erstelle ein Listenobjekt
            int index = worksheet.ListObjects.Add(0, 0, 5, 1, true);
            ListObject listObj = worksheet.ListObjects[index];
            listObj.TableStyleType = TableStyleType.TableStyleLight2;

            // ListObject-Größe ändern
            listObj.Resize(0, 0, 9, 1, true);

            // Speichere die Arbeitsmappe
            workbook.Save("ResizedListObject.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


