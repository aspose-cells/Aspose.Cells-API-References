---
title: "OdsCellFieldCollection.UpdateFieldsValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OdsCellFieldCollection metod. Uppdatera fältvärden till cellerna"
type: docs
url: /sv/net/aspose.cells.ods/odscellfieldcollection/updatefieldsvalue/
---
## OdsCellFieldCollection.UpdateFieldsValue method

Uppdatera fältens värde i cellerna.

```csharp
public void UpdateFieldsValue()
```

### Exempel

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

### Se även

* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


