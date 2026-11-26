---
title: "Enumeración CopyFormatType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.CopyFormatType. Representa el tipo de formato de copia al insertar filas"
type: docs
url: /es/net/aspose.cells/copyformattype/
---
## CopyFormatType enumeration

Representa el tipo de formato de copia al insertar filas.

```csharp
public enum CopyFormatType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| SameAsAbove | `0` | Formatea igual que la fila anterior. |
| SameAsBelow | `1` | Formatea igual que la fila siguiente. |
| Clear | `2` | Borra el formato. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CopyFormatTypeDemo
    {
        public static void CopyFormatTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Llena algunos datos en la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");

            // Crear InsertOptions y establecer CopyFormatType
            InsertOptions insertOptions = new InsertOptions();
            insertOptions.CopyFormatType = CopyFormatType.SameAsAbove;

            // Insertar una fila en la segunda posición con el tipo de formato especificado
            worksheet.Cells.InsertRows(1, 1, insertOptions);

            // Guarda el libro de trabajo
            workbook.Save("CopyFormatTypeExample.xlsx");
            workbook.Save("CopyFormatTypeExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


