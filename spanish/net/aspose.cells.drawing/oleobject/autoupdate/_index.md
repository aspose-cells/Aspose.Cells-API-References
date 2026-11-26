---
title: "OleObject.AutoUpdate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Especifica si el vínculo al OleObject se actualiza automáticamente o no."
type: docs
url: /es/net/aspose.cells.drawing/oleobject/autoupdate/
---
## OleObject.AutoUpdate property

Especifica si el enlace al OleObject se actualiza automáticamente o no.

```csharp
public bool AutoUpdate { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoUpdateDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crear archivos de muestra para la demostración
            string imagePath = "OleObjectExample.jpg";
            string excelPath = "OleObjectExample.xls";
            
            // Crear archivo de imagen de muestra si no existe
            if (!File.Exists(imagePath))
            {
                using (File.Create(imagePath)) { }
            }

            // Crear archivo Excel de muestra si no existe
            if (!File.Exists(excelPath))
            {
                new Workbook().Save(excelPath);
            }

            // Leer datos de la imagen
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Agregar OleObject a la hoja de cálculo
            int oleIndex = sheet.OleObjects.Add(1, 1, 200, 200, imageData);
            Aspose.Cells.Drawing.OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // Establecer propiedades de OleObject
            oleObject.ObjectData = File.ReadAllBytes(excelPath);
            oleObject.ProgID = "Excel.Sheet.8";
            oleObject.DisplayAsIcon = true;
            
            // Demostrar la propiedad AutoUpdate
            oleObject.AutoUpdate = false; // When false, the object won't update automatically when source changes
            
            // Guarda el libro de trabajo
            workbook.Save("OleObjectAutoUpdateDemo.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


