---
title: "WorksheetCollection.BuiltInDocumentProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorksheetCollection. Restituisce una raccolta DocumentProperty che rappresenta tutte le proprietà di documento incorporate del foglio di calcolo"
type: docs
url: /it/net/aspose.cells/worksheetcollection/builtindocumentproperties/
---
## WorksheetCollection.BuiltInDocumentProperties property

Restituisce una raccolta [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) che rappresenta tutte le proprietà di documento incorporate del foglio di calcolo.

```csharp
public BuiltInDocumentPropertyCollection BuiltInDocumentProperties { get; }
```

### Osservazioni

Non è possibile aggiungere una nuova proprietà all'elenco delle proprietà di documento incorporate. È possibile solo ottenere una proprietà incorporata e modificarne il valore. Di seguito è l'elenco dei nomi delle proprietà incorporate:

Title

Subject

Author

Keywords

Comments

Template

Last Author

Revision Number

Application Name

Last Print Date

Creation Date

Last Save Time

Total Editing Time

Number of Pages

Numero di parole

Numero di caratteri

Sicurezza

Categoria

Formato

Gestore

Azienda

Numero di byte

Numero di righe

Numero di paragrafi

Numero di diapositive

Numero di note

Numero di diapositive nascoste

Numero di clip multimediali

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            DocumentProperty authorProperty = workbook.Worksheets.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Document";
            
            Console.WriteLine("Document properties set successfully");
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


