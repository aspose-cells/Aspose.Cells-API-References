---
title: "OleObject.Label"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Obtiene y establece la etiqueta de visualización del objeto ole vinculado"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/label/
---
## OleObject.Label property

Obtiene y establece la etiqueta de visualización del objeto ole vinculado.

```csharp
public string Label { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyLabelDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue un objeto OLE con una etiqueta
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.Label = "label_nameです";

            // Guardar y volver a cargar el libro de trabajo
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            // Verifique la propiedad label
            Workbook loadedWorkbook = new Workbook(outputPath);
            OleObject loadedOleObject = loadedWorkbook.Worksheets[0].OleObjects[0];
            Console.WriteLine("OLE Object Label: " + loadedOleObject.Label);
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


