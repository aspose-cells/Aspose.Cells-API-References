---
title: "Font.ScriptOffset"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene y establece el desplazamiento de super/subíndice en unidades de porcentaje"
type: docs
url: /es/net/aspose.cells/font/scriptoffset/
---
## Font.ScriptOffset property

Obtiene y establece el desplazamiento del script,en unidad de porcentaje

```csharp
public double ScriptOffset { get; set; }
```

### Observaciones

Solo para formas y gráficos.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyScriptOffsetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accede a la celda A1 y establece su valor
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("ScriptOffset Demo");

            // Obtener el estilo y la fuente de la celda
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Establecer ScriptOffset para demostrar el efecto de subíndice/superíndice
            font.ScriptOffset = 10; // Positive for superscript, negative for subscript
            font.IsSuperscript = true; // Enable superscript

            // Aplicar el estilo modificado a la celda
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("FontScriptOffsetDemo.xlsx");

            // Verificar el valor de ScriptOffset
            Console.WriteLine("ScriptOffset value: " + font.ScriptOffset);
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


