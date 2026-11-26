---
title: "Enum OdsCellFieldType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Ods.OdsCellFieldType enum. Representa el tipo de campo de celda de ods"
type: docs
url: /es/net/aspose.cells.ods/odscellfieldtype/
---
## OdsCellFieldType enumeration

Representa el tipo de campo de celda de ODS.

```csharp
public enum OdsCellFieldType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Date | `0` | Fecha actual. |
| SheetName | `1` | El nombre de la hoja. |
| Title | `2` | El nombre del archivo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsCellFieldTypeDemo
    {
        public static void OdsCellFieldTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una OdsCellFieldCollection
            OdsCellFieldCollection odsCellFields = worksheet.Cells.OdsCellFields;

            // Agregar un nuevo OdsCellField para la fecha actual
            int rowIndex = 0;
            int columnIndex = 0;
            string customFormat = "yyyy-mm-dd";
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Date, customFormat);

            // Agregar otro OdsCellField para el nombre de la hoja
            rowIndex = 1;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.SheetName, null);

            // Agregar otro OdsCellField para el título
            rowIndex = 2;
            columnIndex = 0;
            odsCellFields.Add(rowIndex, columnIndex, OdsCellFieldType.Title, null);

            // Actualizar el valor de los campos en las celdas
            odsCellFields.UpdateFieldsValue();

            // Mostrar los valores en la consola
            for (int i = 0; i < odsCellFields.Count; i++)
            {
                OdsCellField field = odsCellFields[i];
                worksheet.Cells[field.Row, field.Column].PutValue($"Field Type: {field.FieldType}, Custom Format: {field.CustomFormat}");
            }

            // Guarda el libro de trabajo
            workbook.Save("OdsCellFieldTypeExample.ods");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


