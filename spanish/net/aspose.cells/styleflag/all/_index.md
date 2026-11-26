---
title: "StyleFlag.All"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicarán todas las propiedades"
type: docs
url: /es/net/aspose.cells/styleflag/all/
---
## StyleFlag.All property

Se aplicarán todas las propiedades.

```csharp
public bool All { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyAllDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear un estilo con fondo rojo sólido
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;

            // Crear una bandera de estilo con la propiedad All establecida en true
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.All = true;

            // Aplicar el estilo a la primera columna
            Column column = cells.Columns[0];
            column.ApplyStyle(style, styleFlag);

            // Verificar que el estilo se aplicó a las celdas de la columna
            Cell cell = cells[0, 0];
            Style appliedStyle = cell.GetStyle();
            
            Console.WriteLine("Pattern: " + appliedStyle.Pattern);
            Console.WriteLine("Color: " + appliedStyle.ForegroundColor);
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


