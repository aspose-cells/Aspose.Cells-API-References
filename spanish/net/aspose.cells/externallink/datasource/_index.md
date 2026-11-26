---
title: "ExternalLink.DataSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalLink. Representa la fuente de datos del enlace externo"
type: docs
url: /es/net/aspose.cells/externallink/datasource/
---
## ExternalLink.DataSource property

Representa la fuente de datos del enlace externo.

```csharp
public string DataSource { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyDataSourceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un enlace externo a otro libro de trabajo
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Cargue el libro de trabajo guardado para verificar los enlaces externos
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Acceda a la propiedad DataSource del enlace externo
            if (loadedWorkbook.Worksheets.ExternalLinks.Count > 0)
            {
                string dataSource = loadedWorkbook.Worksheets.ExternalLinks[0].DataSource;
                Console.WriteLine("External link data source: " + dataSource);
            }
        }
    }
}
```

### Ver también

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


