---
title: "Font.IsBold"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene o establece un valor que indica si la fuente está en negrita"
type: docs
url: /es/net/aspose.cells/font/isbold/
---
## Font.IsBold property

Obtiene o establece un valor que indica si la fuente está en negrita.

```csharp
public bool IsBold { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsBoldDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accede a la celda A1 y establece su valor
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Bold Text Demo");
            
            // Obtener el estilo de la celda y establecer la fuente en negrita
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("FontIsBoldDemo.xlsx");
            
            // Verificar la propiedad negrita
            Workbook loadedWorkbook = new Workbook("FontIsBoldDemo.xlsx");
            Style loadedStyle = loadedWorkbook.Worksheets[0].Cells["A1"].GetStyle();
            Console.WriteLine("IsBold property: " + loadedStyle.Font.IsBold);
        }
    }
}
```

### Ver también

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


