---
title: "OleObject.FullObjectBin"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObject. Obtiene los datos binarios completos del objeto ole incrustado en el archivo de plantilla"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/fullobjectbin/
---
## OleObject.FullObjectBin property

Obtiene los datos binarios completos del objeto ole incrustado en el archivo de plantilla.

```csharp
public byte[] FullObjectBin { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectPropertyFullObjectBinDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un objeto OLE a la hoja de cálculo
            byte[] objectData = File.ReadAllBytes("example.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, objectData, "docx");
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Establecer algunas propiedades para el objeto OLE
            oleObject.FileFormatType = FileFormatType.Docx;
            oleObject.ObjectData = objectData;
            oleObject.IsAutoSize = true;

            // Obtener los datos FullObjectBin (propiedad de solo lectura)
            byte[] fullObjectBinData = oleObject.FullObjectBin;
            Console.WriteLine("FullObjectBin data length: " + (fullObjectBinData != null ? fullObjectBinData.Length.ToString() : "null"));

            // Demostrar el uso de FullObjectBin guardándolo en un archivo
            if (fullObjectBinData != null && fullObjectBinData.Length > 0)
            {
                File.WriteAllBytes("FullObjectBinData.bin", fullObjectBinData);
                Console.WriteLine("Saved FullObjectBin data to file.");
            }

            // Crear otro libro de trabajo para demostrar la lectura del objeto OLE
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];

            // Agregar el objeto OLE desde los datos FullObjectBin
            if (fullObjectBinData != null)
            {
                int newOleObjectIndex = worksheet2.OleObjects.Add(10, 10, 200, 200, fullObjectBinData, "docx");
                Console.WriteLine("Added new OLE object using FullObjectBin data.");
            }

            // Guardar los libros de trabajo
            workbook.Save("OleObjectWithFullObjectBin.xlsx");
            workbook2.Save("OleObjectFromFullObjectBin.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


