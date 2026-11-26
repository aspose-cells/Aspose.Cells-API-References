---
title: "OdsCellFieldCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método OdsCellFieldCollection. Agrega un campo"
type: docs
url: /es/net/aspose.cells.ods/odscellfieldcollection/add/
---
## OdsCellFieldCollection.Add method

Agrega un campo.

```csharp
public int Add(int row, int column, OdsCellFieldType fieldType, string format)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |
| fieldType | OdsCellFieldType | El tipo del campo. |
| formato | String | El formato numérico del campo. |

### Ejemplos

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

            // Agregar diferentes tipos de campos
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-MM-dd");
            odsCellFields.Add(1, 1, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 2, OdsCellFieldType.Title, "SampleTitle");

            odsCellFields.UpdateFieldsValue();
            workbook.Save("OdsCellFieldsDemo.ods");
        }
    }
}
```

### Ver también

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellFieldCollection](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


