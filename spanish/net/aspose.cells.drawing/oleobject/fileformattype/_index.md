---
title: "OleObject.FileFormatType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Obtiene y establece el tipo de archivo de los datos del objeto ole incrustado"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/fileformattype/
---
## OleObject.FileFormatType property

Obtiene y establece el tipo de archivo de los datos del objeto ole incrustado

```csharp
public FileFormatType FileFormatType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue un objeto OLE a la hoja de cálculo (sin datos de archivo)
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, null);
            
            // Obtenga el objeto OLE agregado
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            
            // Establezca y muestre el tipo de formato de archivo
            oleObject.FileFormatType = FileFormatType.Docm;
            Console.WriteLine("OLE Object File Format Type: " + oleObject.FileFormatType);
            
            // Guarda el libro de trabajo
            workbook.Save("OleObjectFileFormatTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FileFormatType](../../../aspose.cells/fileformattype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


