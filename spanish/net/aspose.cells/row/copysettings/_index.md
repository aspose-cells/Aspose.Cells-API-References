---
title: "Row.CopySettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Row. Copia la configuración de la fila como estilo, altura, visibilidad, etc."
type: docs
url: /es/net/aspose.cells/row/copysettings/
---
## Row.CopySettings method

Copia la configuración de la fila, como estilo, altura, visibilidad, ...etc.

```csharp
public void CopySettings(Row source, bool checkStyle)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| origen | Row | la fila fuente cuya configuración será copiada a esta |
| checkStyle | Booleano | si verifica y recopila el estilo. Sólo tiene efecto y es necesario cuando dos objetos fila pertenecen a diferentes libros de trabajo y los estilos de los dos libros son diferentes. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodCopySettingsWithRowBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear y aplicar estilo a la fila fuente
            Row sourceRow = worksheet.Cells.Rows[0];
            Style sourceStyle = workbook.CreateStyle();
            sourceStyle.BackgroundColor = Color.Blue;
            sourceRow.ApplyStyle(sourceStyle, new StyleFlag { All = true });
            sourceRow.Height = 25;
            sourceRow.IsHidden = false;

            // Crear fila objetivo
            Row targetRow = worksheet.Cells.Rows[1];
            
            // Demostrar CopySettings con copyStyle=true
            targetRow.CopySettings(sourceRow, true);

            // Verificar que la configuración fue copiada
            Console.WriteLine($"Target row height: {targetRow.Height}");
            Console.WriteLine($"Target row is hidden: {targetRow.IsHidden}");

            workbook.Save("RowCopySettingsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


