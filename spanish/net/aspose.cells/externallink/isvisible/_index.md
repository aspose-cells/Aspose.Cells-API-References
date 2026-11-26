---
title: "ExternalLink.IsVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalLink. Indica si este enlace externo es visible en MS Excel"
type: docs
url: /es/net/aspose.cells/externallink/isvisible/
---
## ExternalLink.IsVisible property

Indica si este enlace externo es visible en MS Excel.

```csharp
public bool IsVisible { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con enlaces externos
            Workbook workbook = new Workbook();
            
            // Agregar algunos datos a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("External Link Demo");
            
            // Crear un nuevo libro de trabajo para usar como fuente de enlace externo
            Workbook externalWorkbook = new Workbook();
            externalWorkbook.Worksheets[0].Cells["A1"].PutValue(100);
            externalWorkbook.Save("external_data.xlsx");
            
            // Agregar una referencia de enlace externo
            workbook.Worksheets[0].Cells["B1"].Formula = "='[external_data.xlsx]Sheet1'!A1";
            
            // Verificar enlaces externos (se crearán automáticamente al cargar fórmulas)
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link visibility: {link.IsVisible}");
                Console.WriteLine($"External link data source: {link.DataSource}");
            }
            
            // Crear otro libro de trabajo para demostrar la carga de un archivo existente
            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("=SUM([example.xls]Sheet1!A1:A10)");
            
            // Guardar y recargar para demostrar los enlaces externos
            workbook2.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Verificar enlaces externos en el libro de trabajo cargado
            foreach (ExternalLink link in loadedWorkbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link URL: {link.DataSource}, Visible: {link.IsVisible}");
            }
        }
    }
}
```

### Ver también

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


