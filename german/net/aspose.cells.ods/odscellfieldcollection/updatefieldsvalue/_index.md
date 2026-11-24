---
title: "OdsCellFieldCollection.UpdateFieldsValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OdsCellFieldCollection-Methode. Aktualisiert den Feldwert in den Zellen"
type: docs
url: /de/net/aspose.cells.ods/odscellfieldcollection/updatefieldsvalue/
---
## OdsCellFieldCollection.UpdateFieldsValue method

Aktualisiert den Feldwert in den Zellen.

```csharp
public void UpdateFieldsValue()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldCollectionMethodUpdateFieldsValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            OdsCellFieldCollection odsCellFields = cells.OdsCellFields;

            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-MM-dd");
            odsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 2, OdsCellFieldType.Title, null);

            odsCellFields.UpdateFieldsValue();

            workbook.Save("OdsCellFieldCollectionExample.ods");
        }
    }
}
```

### Siehe auch

* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


