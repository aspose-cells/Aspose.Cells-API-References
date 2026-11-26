---
title: "OleObject.IsAutoSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. True indica que el tamaño del objeto ole se cambiará automáticamente al tamaño de la instantánea del contenido incrustado cuando el objeto ole se active"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/isautosize/
---
## OleObject.IsAutoSize property

True indica que el tamaño del objeto ole se cambiará automáticamente al tamaño de la instantánea del contenido incrustado cuando se active el objeto ole.

```csharp
public bool IsAutoSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un objeto OLE (usando datos del archivo como matriz de bytes)
            byte[] oleData = System.IO.File.ReadAllBytes(@"C:\example\test.docx");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, oleData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];

            // Establecer y demostrar la propiedad IsAutoSize
            oleObject.IsAutoSize = true;
            Console.WriteLine("OLE Object AutoSize initially: " + oleObject.IsAutoSize);

            // Cambiar la propiedad
            oleObject.IsAutoSize = false;
            Console.WriteLine("OLE Object AutoSize after change: " + oleObject.IsAutoSize);

            // Guarda el libro de trabajo
            workbook.Save("OleObjectIsAutoSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


