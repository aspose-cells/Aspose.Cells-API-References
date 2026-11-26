---
title: "OleObject.ObjectData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Representa los datos del objeto ole incrustado como una matriz de bytes"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/objectdata/
---
## OleObject.ObjectData property

Representa los datos del objeto ole incrustado como una matriz de bytes.

```csharp
public byte[] ObjectData { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            var workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            var worksheet = workbook.Worksheets[0];
            
            // Rutas de archivo de ejemplo (reemplácelas con rutas reales en su entorno)
            string imagePath = "logo.jpg";
            string oleDataPath = "test.xls";

            // Agregar objeto OLE con datos de imagen iniciales
            int oleIndex = worksheet.OleObjects.Add(10, 10, 300, 200, File.ReadAllBytes(imagePath));
            
            // Modificar los datos del objeto OLE
            worksheet.OleObjects[oleIndex].ObjectData = File.ReadAllBytes(oleDataPath);
            
            // Guarda el libro de trabajo
            workbook.Save("OleObjectDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("OLE object demo created successfully.");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


