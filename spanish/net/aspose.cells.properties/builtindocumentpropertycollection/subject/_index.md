---
title: "BuiltInDocumentPropertyCollection.Subject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Obtiene o establece el asunto del documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/subject/
---
## BuiltInDocumentPropertyCollection.Subject property

Obtiene o establece el asunto del documento.

```csharp
public string Subject { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertySubjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer propiedades de documento incorporadas
            workbook.BuiltInDocumentProperties.Subject = "LiteraTest";
            workbook.BuiltInDocumentProperties.Title = "LiteraTest";

            // Guarda el libro de trabajo
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Cargue el libro de trabajo guardado para verificar las propiedades
            using (Workbook loadedWorkbook = new Workbook(outputPath))
            {
                string subject = loadedWorkbook.BuiltInDocumentProperties.Subject;
                string title = loadedWorkbook.BuiltInDocumentProperties.Title;

                Console.WriteLine("Subject: " + subject);
                Console.WriteLine("Title: " + title);
            }
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


