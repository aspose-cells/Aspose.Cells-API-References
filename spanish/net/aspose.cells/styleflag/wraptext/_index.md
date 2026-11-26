---
title: "StyleFlag.WrapText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración de ajuste de texto"
type: docs
url: /es/net/aspose.cells/styleflag/wraptext/
---
## StyleFlag.WrapText property

Se aplicará la configuración de ajuste de texto.

```csharp
public bool WrapText { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyWrapTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo con ajuste de texto habilitado
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Crear una bandera de estilo y habilitar la bandera WrapText
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;

            // Aplicar el estilo a la celda A1 con las banderas especificadas
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap in the cell");
            worksheet.Cells.ApplyStyle(style, flag);

            // Ajustar automáticamente la altura de la fila para ver el texto ajustado
            worksheet.AutoFitRow(0);

            // Guarda el libro de trabajo
            workbook.Save("WrapTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


