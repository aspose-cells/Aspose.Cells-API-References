---
title: "OleObject.DisplayAsIcon"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Verdadero si el objeto especificado se muestra como un ícono y la imagen no se cambiará automáticamente"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/displayasicon/
---
## OleObject.DisplayAsIcon property

True si el objeto especificado se muestra como un ícono y la imagen no se cambiará automáticamente.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue un objeto OLE (PDF) a la hoja de cálculo
            byte[] pdfData = File.ReadAllBytes("example.pdf");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfData);
            
            // Obtenga el objeto OLE
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.ProgID = "AcroExch.Document.DC";
            
            // Demuestre la propiedad DisplayAsIcon
            oleObject.DisplayAsIcon = true; // Show as icon
            // oleObject.DisplayAsIcon = false; // Mostrar contenido si es posible
            
            // Guarda el libro de trabajo
            workbook.Save("OleObjectDisplayAsIconDemo.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


