---
title: "BuiltInDocumentPropertyCollection.Bytes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà BuiltInDocumentPropertyCollection. Rappresenta una stima del numero di byte nel documento"
type: docs
url: /it/net/aspose.cells.properties/builtindocumentpropertycollection/bytes/
---
## BuiltInDocumentPropertyCollection.Bytes property

Rappresenta una stima del numero di byte nel documento.

```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Bytes { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class BuiltInDocumentPropertyCollectionPropertyBytesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi alle proprietà del documento integrate
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Visualizza il valore corrente di Bytes (stima della dimensione del documento)
            Console.WriteLine("Current Bytes value: " + properties.Bytes);

            // Aggiungi del contenuto per influenzare la dimensione
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample data to increase document size");
            for (int i = 2; i <= 100; i++)
            {
                worksheet.Cells["A" + i].PutValue("Line " + i);
            }

            // Aggiorna manualmente la proprietà Bytes (anche se normalmente verrebbe calcolata automaticamente)
            properties.Bytes = 5000;
            Console.WriteLine("Updated Bytes value: " + properties.Bytes);

            // Salva la cartella di lavoro per vedere la proprietà nel file salvato
            workbook.Save("PropertyBytesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


