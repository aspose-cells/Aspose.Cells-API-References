---
title: "OdsCellField.Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsCellField. Obtiene y establece el índice de fila de la celda"
type: docs
url: /es/net/aspose.cells.ods/odscellfield/row/
---
## OdsCellField.Row property

Obtiene y establece el índice de fila de la celda.

```csharp
public int Row { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;
            
            // Agregar campos con diferentes tipos
            odsCellFields.Add(0, 0, OdsCellFieldType.Date, "yyyy-mm-dd");
            odsCellFields.Add(1, 0, OdsCellFieldType.SheetName, null);
            odsCellFields.Add(2, 0, OdsCellFieldType.Title, null);
            
            odsCellFields.UpdateFieldsValue();

            // Demostrar el uso de la propiedad Row
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                int row = field.Row; // Using Row property
                worksheet.Cells[row, 1].PutValue($"Row: {row}, Type: {field.FieldType}");
            }

            workbook.Save("OdsCellFieldRowDemo.ods");
        }
    }
}
```

### Ver también

* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


