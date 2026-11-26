---
title: "OleObject.ObjectSourceFullName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Devuelve el nombre completo de origen del archivo fuente para el objeto OLE vinculado"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/objectsourcefullname/
---
## OleObject.ObjectSourceFullName property

Devuelve el nombre completo de origen del archivo fuente para el objeto OLE vinculado.

```csharp
public string ObjectSourceFullName { get; set; }
```

### Observaciones

Solo admite establecer el nombre completo de origen cuando el tipo de archivo es OleFileType.Unknown. Como archivos wav, avi, etc.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectSourceFullNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un objeto OLE (usando datos del archivo como matriz de bytes)
            byte[] fileData = System.IO.File.ReadAllBytes("test.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Establecer y obtener ObjectSourceFullName
            oleObject.ObjectSourceFullName = "C:\\Temp\\source.docx";
            Console.WriteLine("OLE Object Source Full Name: " + oleObject.ObjectSourceFullName);

            // Guarda el libro de trabajo
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


