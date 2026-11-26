---
title: "OleObject.IsLink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Devuelve true si el OleObject enlaza al archivo"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/islink/
---
## OleObject.IsLink property

Devuelve verdadero si el OleObject enlaza al archivo.

```csharp
public bool IsLink { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsLinkDemo
    {
        public static void Run()
        {
            // Cargar el libro de trabajo de origen
            Workbook workbook = new Workbook("example.xlsm");

            // Procesar cada hoja de cálculo
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                // Procesar cada objeto OLE en la hoja de cálculo
                foreach (Aspose.Cells.Drawing.OleObject ole in worksheet.OleObjects)
                {
                    // Omitir si el objeto OLE no está enlazado
                    if (!ole.IsLink)
                    {
                        Console.WriteLine("Skipping embedded OLE object");
                        continue;
                    }

                    // Mostrar y modificar la ruta del archivo enlazado
                    Console.WriteLine("Original linked file: " + ole.ObjectSourceFullName);
                    string newPath = ole.ObjectSourceFullName.Replace("C:", "D:");
                    ole.ObjectSourceFullName = newPath;
                    Console.WriteLine("Modified linked file: " + ole.ObjectSourceFullName);
                }
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("modified_example.xlsm");
            Console.WriteLine("File saved with updated OLE links.");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


