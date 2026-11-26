---
title: "Workbook.FileName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Workbook property. Obtiene y establece el nombre de archivo actual"
type: docs
url: /es/net/aspose.cells/workbook/filename/
---
## Workbook.FileName property

Obtiene y establece el nombre actual del archivo.

```csharp
public string FileName { get; set; }
```

### Observaciones

Si el archivo se abre mediante un flujo y existen referencias a fórmulas externas, por favor establezca el nombre del archivo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyFileNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Establecer la propiedad del nombre de archivo
            wb.FileName = "SampleWorkbook.xlsx";
            
            // Agregar algunos datos para demostrar la funcionalidad
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Workbook FileName Demo");
            sheet.Cells["A2"].PutValue("Current FileName:");
            sheet.Cells["B2"].PutValue(wb.FileName);
            
            // Guarda el libro de trabajo
            wb.Save(wb.FileName);
            
            Console.WriteLine($"Workbook created with filename: {wb.FileName}");
            
            // Demostrar el cambio del nombre de archivo
            Workbook wb2 = new Workbook();
            wb2.FileName = "ChangedName.xlsx";
            Console.WriteLine($"New workbook filename set to: {wb2.FileName}");
            
            // Demostrar el uso de enlaces externos
            if (wb.Worksheets.ExternalLinks.Count > 0)
            {
                string externalSource = wb.Worksheets.ExternalLinks[0].DataSource;
                wb2.FileName = externalSource;
                Console.WriteLine($"Updated filename to external source: {wb2.FileName}");
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


