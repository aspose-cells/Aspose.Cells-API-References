---
title: "OdsCellFieldCollection.UpdateFieldsValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método OdsCellFieldCollection. Actualiza el valor de los campos en las celdas"
type: docs
url: /es/net/aspose.cells.ods/odscellfieldcollection/updatefieldsvalue/
---
## OdsCellFieldCollection.UpdateFieldsValue method

Actualiza el valor de los campos en las celdas.

```csharp
public void UpdateFieldsValue()
```

### Ejemplos

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

### Ver también

* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


