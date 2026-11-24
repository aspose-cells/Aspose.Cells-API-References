---
title: "OdsCellFieldCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsCellFieldCollection-Methode. Fügt ein Feld hinzu"
type: docs
url: /de/net/aspose.cells.ods/odscellfieldcollection/add/
---
## OdsCellFieldCollection.Add method

Fügt ein Feld hinzu.

```csharp
public int Add(int row, int column, OdsCellFieldType fieldType, string format)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Der Zeilenindex. |
| column | Int32 | Der Spaltenindex. |
| fieldType | OdsCellFieldType | Der Typ des Feldes. |
| Format | String | Das Zahlenformat des Feldes. |

### Beispiele

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

            // Unterschiedliche Feldtypen hinzufügen
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-MM-dd");
            odsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 2, OdsCellFieldType.Title, "SampleTitle");

            odsCellFields.UpdateFieldsValue();
            workbook.Save("OdsCellFieldsDemo.ods");
        }
    }
}
```

### Siehe auch

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


