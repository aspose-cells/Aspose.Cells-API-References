---
title: "OleObject.AutoLoad"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Especifica si la aplicación host del objeto incrustado debe ser llamada para cargar los datos del objeto automáticamente cuando se abre el libro de trabajo principal."
type: docs
url: /es/net/aspose.cells.drawing/oleobject/autoload/
---
## OleObject.AutoLoad property

Especifica si la aplicación host del objeto incrustado debe ser llamada para cargar los datos del objeto automáticamente cuando se abre el libro de trabajo principal.

```csharp
public bool AutoLoad { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoLoadDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar un OleObject a la hoja de cálculo
            int oleNumber = sheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            
            // Establecer propiedades de OleObject
            OleObject ole = sheet.OleObjects[oleNumber];
            ole.ProgID = "Excel.Sheet";
            ole.ObjectData = new byte[0];
            
            // Demostrar la propiedad AutoLoad
            ole.AutoLoad = true; // Automatically load the OleObject when the workbook opens
            
            // Guarda el libro de trabajo
            workbook.Save("OleObjectAutoLoadDemo.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


