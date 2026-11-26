---
title: "StyleFlag.NumberFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración del formato numérico"
type: docs
url: /es/net/aspose.cells/styleflag/numberformat/
---
## StyleFlag.NumberFormat property

Se aplicará la configuración de formato numérico.

```csharp
public bool NumberFormat { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyNumberFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Establecer valor de celda
            sheet.Cells[0, 0].Value = 1234.56;
            
            // Crear estilo de formato numérico personalizado
            Style style = workbook.CreateStyle();
            style.Custom = "_-€ #,##0.00;[Red]_-€ -#,##0.00";
            
            // Aplicar solo el formato numérico usando StyleFlag
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            
            // Aplicar el estilo al rango de celdas (calificar completamente el tipo Range)
            Aspose.Cells.Range range = sheet.Cells.CreateRange(0, 0, 1, 1);
            range.ApplyStyle(style, styleFlag);
            
            // Guardar y verificar
            workbook.Save("output_number_format.ods");
            
            // Recargar para verificar
            Workbook verifyWorkbook = new Workbook("output_number_format.ods");
            Worksheet verifySheet = verifyWorkbook.Worksheets[0];
            Console.WriteLine("Applied Number Format: " + verifySheet.Cells["A1"].GetStyle().Custom);
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


