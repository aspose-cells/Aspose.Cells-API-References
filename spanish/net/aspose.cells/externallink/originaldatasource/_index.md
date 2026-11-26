---
title: "ExternalLink.OriginalDataSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ExternalLink. Representa la fuente de datos almacenada del enlace externo"
type: docs
url: /es/net/aspose.cells/externallink/originaldatasource/
---
## ExternalLink.OriginalDataSource property

Representa la fuente de datos almacenada del enlace externo.

```csharp
public string OriginalDataSource { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyOriginalDataSourceDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con enlaces externos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar enlace externo
            worksheet.Cells["A1"].Formula = "='https://arcusventures.sharepoint.com/Fund II/[example.xlsx]Sheet1'!A1";
            
            // Modificar rutas de enlaces externos
            for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
            {
                string originalLink = workbook.Worksheets.ExternalLinks[i].OriginalDataSource;
                string modifiedLink = originalLink.Replace(
                    @"https://arcusventures.sharepoint.com/Fund II/", 
                    @"/sites/shared/shared documents/Fund II/");
                
                workbook.Worksheets.ExternalLinks[i].OriginalDataSource = modifiedLink;
            }
            
            // Verificar los cambios
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine("Modified Link: " + link.OriginalDataSource);
            }
        }
    }
}
```

### Ver también

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


