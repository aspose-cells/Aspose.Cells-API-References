---
title: "Name.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Name. Obtiene el texto del nombre del objeto"
type: docs
url: /es/net/aspose.cells/name/text/
---
## Name.Text property

Obtiene el texto del nombre del objeto.

```csharp
public string Text { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un rango con nombre
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Establecer y mostrar la propiedad Text
            namedRange.Text = "MyCustomName";
            Console.WriteLine("Named range text: " + namedRange.Text);
            
            // Guarda el libro de trabajo
            workbook.Save("NamedRangeExample.xlsx");
        }
    }
}
```

### Ver también

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


