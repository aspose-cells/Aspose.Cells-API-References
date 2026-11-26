---
title: "InsertOptions.CopyFormatType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad InsertOptions."
type: docs
url: /es/net/aspose.cells/insertoptions/copyformattype/
---
## InsertOptions.CopyFormatType property

```csharp
public CopyFormatType CopyFormatType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InsertOptionsPropertyCopyFormatTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer valores y formato para la demostración
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["A3"].PutValue("Item2");

            // Crear InsertOptions y establecer CopyFormatType
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.SameAsAbove;

            // Insertar fila con formato de arriba
            worksheet.Cells.InsertRows(2, 1, options);

            // Guardar el resultado
            workbook.Save("InsertWithFormatting.xlsx");
        }
    }
}
```

### Ver también

* enum [CopyFormatType](../../copyformattype/)
* class [InsertOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


