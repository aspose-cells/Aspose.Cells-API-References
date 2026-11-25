---
title: "DocumentProperty.IsGeneratedName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DocumentProperty. Restituisce true se questa proprietà non ha un nome nell'archivio OLE2 ed è stato generato un nome univoco solo per l'API pubblica"
type: docs
url: /it/net/aspose.cells.properties/documentproperty/isgeneratedname/
---
## DocumentProperty.IsGeneratedName property

Restituisce true se questa proprietà non ha un nome nello storage OLE2 ed è stato generato un nome univoco solo per l'API pubblica.

```csharp
public bool IsGeneratedName { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyPropertyIsGeneratedNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle proprietà del documento integrate
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;
            
            // Accedi alle proprietà documento personalizzate per aggiungere
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Aggiungi una proprietà personalizzata
            DocumentProperty customProperty = customProperties.Add("CustomProperty", "Test Value");
            
            // Visualizza IsGeneratedName per la proprietà incorporata
            DocumentProperty authorProperty = properties["Author"];
            Console.WriteLine("Author property IsGeneratedName: " + authorProperty.IsGeneratedName);
            
            // Visualizza IsGeneratedName per la proprietà personalizzata
            Console.WriteLine("Custom property IsGeneratedName: " + customProperty.IsGeneratedName);

            // Crea uno scenario in cui una proprietà potrebbe avere un nome generato
            // (Nota: In pratica, IsGeneratedName è di sola lettura e impostato internamente da Aspose.Cells)
            DocumentProperty generatedNameProperty = properties["_PID_GUID"];
            if (generatedNameProperty != null)
            {
                Console.WriteLine("Generated name property IsGeneratedName: " + generatedNameProperty.IsGeneratedName);
            }

            // Salva la cartella di lavoro
            workbook.Save("PropertyIsGeneratedNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


