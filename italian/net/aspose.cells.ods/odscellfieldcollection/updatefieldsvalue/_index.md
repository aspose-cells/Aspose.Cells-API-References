---
title: "OdsCellFieldCollection.UpdateFieldsValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo OdsCellFieldCollection. Aggiorna il valore dei campi nelle celle"
type: docs
url: /it/net/aspose.cells.ods/odscellfieldcollection/updatefieldsvalue/
---
## OdsCellFieldCollection.UpdateFieldsValue method

Aggiorna il valore dei campi nelle celle.

```csharp
public void UpdateFieldsValue()
```

### Esempi

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

### Vedi anche

* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


