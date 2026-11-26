---
title: "Style.IsBorderApplied"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Indica si se debe aplicar el formato de borde"
type: docs
url: /es/net/aspose.cells/style/isborderapplied/
---
## Style.IsBorderApplied property

Indica si se debe aplicar el formato de borde.

```csharp
public bool IsBorderApplied { get; set; }
```

### Observaciones

Solo para estilo con nombre.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsBorderAppliedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un estilo personalizado
            Style style = workbook.CreateStyle();
            
            // Aplicar la configuración de borde al estilo
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Black;
            
            // Verificar si el borde está aplicado
            Console.WriteLine("IsBorderApplied before setting: " + style.IsBorderApplied);
            
            // Establezca explícitamente IsBorderApplied a true
            style.IsBorderApplied = true;
            
            // Aplicar el estilo a una celda
            worksheet.Cells["A1"].SetStyle(style);
            
            // Verificar la aplicación del borde
            Console.WriteLine("IsBorderApplied after setting: " + style.IsBorderApplied);
            
            // Guarda el libro de trabajo
            workbook.Save("IsBorderAppliedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


