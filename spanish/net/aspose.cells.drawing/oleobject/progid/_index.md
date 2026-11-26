---
title: "OleObject.ProgID"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Obtiene o establece el ProgID del objeto OLE"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/progid/
---
## OleObject.ProgID property

Obtiene o establece el ProgID del objeto OLE.

```csharp
public string ProgID { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyProgIDDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un objeto OLE a la hoja de cálculo
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0], "test.pdf");
            OleObject ole = worksheet.OleObjects[oleIndex];
            
            // Establecer el ProgID para el objeto OLE
            ole.ProgID = "AcroExch.Document.DC";
            
            // Mostrar el ProgID
            Console.WriteLine("OLE Object ProgID: " + ole.ProgID);

            // Guarda el libro de trabajo
            workbook.Save("OleObjectProgIDDemo.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


