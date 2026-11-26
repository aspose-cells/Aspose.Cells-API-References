---
title: "Style.IsFontApplied"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Indique si se debe aplicar el formato de fuente"
type: docs
url: /es/net/aspose.cells/style/isfontapplied/
---
## Style.IsFontApplied property

Indica si se debe aplicar el formato de fuente.

```csharp
public bool IsFontApplied { get; set; }
```

### Observaciones

Solo para estilo con nombre.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFontAppliedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceda a una celda de la hoja de cálculo
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            
            // Obtener el estilo de la celda
            Style style = cell.GetStyle();
            
            // Aplica la configuración de fuente
            style.Font.Name = "Times New Roman";
            style.Font.Size = 14;
            style.Font.Color = Color.Blue;
            
            // Habilitar aplicación de fuente
            style.IsFontApplied = true;
            
            // Establecer el estilo modificado de nuevo en la celda
            cell.SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("FontAppliedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


