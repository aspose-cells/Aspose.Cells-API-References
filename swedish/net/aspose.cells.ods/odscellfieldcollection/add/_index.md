---
title: "OdsCellFieldCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsCellFieldCollection-metod. Lägger till ett fält"
type: docs
url: /sv/net/aspose.cells.ods/odscellfieldcollection/add/
---
## OdsCellFieldCollection.Add method

Lägger till ett fält.

```csharp
public int Add(int row, int column, OdsCellFieldType fieldType, string format)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindexet. |
| column | Int32 | Kolumnindexet. |
| fieldType | OdsCellFieldType | Typen av fältet. |
| format | String | Nummerformatet för fältet. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionMethodAddWithInt32Int32OdsCellFieldTypStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Lägg till olika typer av fält
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-MM-dd");
            odsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 2, OdsCellFieldType.Title, "SampleTitle");

            odsCellFields.UpdateFieldsValue();
            workbook.Save("OdsCellFieldsDemo.ods");
        }
    }
}
```

### Se även

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


