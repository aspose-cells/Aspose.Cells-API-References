---
title: "AutoFitterOptions.AutoFitMergedCellsType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoFitterOptions. Obtiene y establece el tipo de ajuste automático de la altura de fila de celdas combinadas"
type: docs
url: /es/net/aspose.cells/autofitteroptions/autofitmergedcellstype/
---
## AutoFitterOptions.AutoFitMergedCellsType property

Obtiene y establece el tipo de ajuste automático de la altura de fila de celdas fusionadas.

```csharp
public AutoFitMergedCellsType AutoFitMergedCellsType { get; set; }
```

### Observaciones

Excel, por defecto, ignora las celdas combinadas al ajustar la altura de la fila, por lo que Aspose.Cells funciona como el valor predeterminado de MS Excel. Por favor, establezca este tipo para cambiar la forma de ajustar automáticamente la altura de fila de celdas combinadas.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyAutoFitMergedCellsTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer datos de muestra y combinar celdas
            worksheet.Cells["A1"].PutValue("This is a sample text for merged cells auto-fit demonstration");
            worksheet.Cells.Merge(0, 0, 3, 2); // Merge A1:B3

            // Ajustar filas con AutoFitMergedCellsType.EachLine
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // Ajustar columnas con AutoFitMergedCellsType.EachLine
            worksheet.AutoFitColumns(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
            });

            // Guarda el libro de trabajo
            workbook.Save("AutoFitMergedCellsDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [AutoFitMergedCellsType](../../autofitmergedcellstype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


