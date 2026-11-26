---
title: "CopyOptions.ColumnCharacterWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de CopyOptions. Indica si se copia el ancho de columna en unidades de caracteres"
type: docs
url: /es/net/aspose.cells/copyoptions/columncharacterwidth/
---
## CopyOptions.ColumnCharacterWidth property

Indica si se copia el ancho de columna en unidades de caracteres.

```csharp
public bool ColumnCharacterWidth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyColumnCharacterWidthDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo de origen con datos de muestra
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // Establezca el ancho de columna en caracteres para la demostración
            srcSheet.Cells.SetColumnWidth(0, 20); // 20 characters wide
            
            // Agregar algunos datos de ejemplo
            srcSheet.Cells["A1"].PutValue("Sample Text");
            srcSheet.Cells["A2"].PutValue("Another Sample");
            
            // Cree un libro de trabajo de destino
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Copie con ColumnCharacterWidth establecido en true
            destSheet.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = true
            });
            
            // Guardar el resultado
            destWorkbook.Save("output_with_column_width.xlsx", SaveFormat.Xlsx);
            
            // Para comparar, copie sin ColumnCharacterWidth
            Workbook destWorkbook2 = new Workbook();
            Worksheet destSheet2 = destWorkbook2.Worksheets[0];
            
            destSheet2.Copy(srcSheet, new CopyOptions()
            {
                ColumnCharacterWidth = false
            });
            
            destWorkbook2.Save("output_without_column_width.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


