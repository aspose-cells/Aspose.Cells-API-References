---
title: "OleObject.ClassIdentifier"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Obtiene y establece el identificador de clase del objeto incrustado. Indica qué aplicación abre el archivo incrustado"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/classidentifier/
---
## OleObject.ClassIdentifier property

Obtiene y establece el identificador de clase del objeto incrustado. Significa qué aplicación abre el archivo incrustado.

```csharp
public byte[] ClassIdentifier { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyClassIdentifierDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Matriz de bytes de ejemplo para ClassIdentifier (normalmente esto sería un ID de clase real)
            byte[] classId = new byte[] { 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 
                                         0x09, 0x0A, 0x0B, 0x0C, 0x0D, 0x0E, 0x0F, 0x10 };

            // Agregar un objeto OLE con datos de ejemplo
            int oleIndex = sheet.OleObjects.Add(10, 10, 200, 100, new byte[100]);
            OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // Establecer la propiedad ClassIdentifier
            oleObject.ClassIdentifier = classId;
            oleObject.ProgID = "Excel.Sheet.12";
            oleObject.DisplayAsIcon = true;

            // Guarda el libro de trabajo
            workbook.Save("OleObjectDemo.xlsx");

            // Cargar el libro de trabajo guardado para verificar el ClassIdentifier
            Workbook loadedWorkbook = new Workbook("OleObjectDemo.xlsx");
            OleObject loadedOle = loadedWorkbook.Worksheets[0].OleObjects[0];
            
            // Verifique que se conservó el ClassIdentifier
            Console.WriteLine("ClassIdentifier length: " + loadedOle.ClassIdentifier.Length);
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


