---
title: "Worksheet.OleObjects"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Representa una colección de OleObject en una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheet/oleobjects/
---
## Worksheet.OleObjects property

Representa una colección de [`OleObject`](../../../aspose.cells.drawing/oleobject/) en una hoja de cálculo.

```csharp
public OleObjectCollection OleObjects { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOleObjectsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un OleObject a la hoja de cálculo
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(@"C:\temp\example.xlsx"));
            OleObject ole = worksheet.OleObjects[oleObjectIndex];
            
            // Modificar propiedades de OleObject
            ole.ObjectSourceFullName = @"C:\temp\modified.xlsx";
            ole.FileFormatType = FileFormatType.Xlsx;

            // Guarda el libro de trabajo
            workbook.Save(@"C:\temp\output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [OleObjectCollection](../../../aspose.cells.drawing/oleobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


