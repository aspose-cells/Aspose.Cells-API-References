---
title: "PdfSaveOptions.CustomPropertiesExport"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSaveOptions. Obtient ou définit une valeur déterminant la façon dont CustomDocumentPropertyCollection sont exportées vers le fichier PDF. La valeur par défaut est None"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/custompropertiesexport/
---
## PdfSaveOptions.CustomPropertiesExport property

Obtient ou définit une valeur déterminant la façon dont [`CustomDocumentPropertyCollection`](../../../aspose.cells.properties/customdocumentpropertycollection/) sont exportées vers le fichier PDF. La valeur par défaut est None.

```csharp
public PdfCustomPropertiesExport CustomPropertiesExport { get; set; }
```

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyCustomPropertiesExportDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose");
            worksheet.Cells["A2"].PutValue("Sample PDF Export");

            workbook.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.CustomDocumentProperties.Add("Subject", "Aspose.Cells Example");

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;

            workbook.Save("PdfCustomPropertiesExportDemo.pdf", saveOptions);
        }
    }
}
```

### Voir aussi

* enum [PdfCustomPropertiesExport](../../../aspose.cells.rendering/pdfcustompropertiesexport/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


