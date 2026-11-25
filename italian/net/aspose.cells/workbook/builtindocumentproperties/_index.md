---
title: "Workbook.BuiltInDocumentProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà del workbook. Restituisce una raccolta DocumentProperty che rappresenta tutte le proprietà di documento integrate del foglio di calcolo"
type: docs
url: /it/net/aspose.cells/workbook/builtindocumentproperties/
---
## Workbook.BuiltInDocumentProperties property

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
    public class WorkbookPropertyBuiltInDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi e modifica le proprietà di documento integrate
            DocumentProperty authorProperty = workbook.BuiltInDocumentProperties["Author"];
            authorProperty.Value = "John Smith";
            
            DocumentProperty titleProperty = workbook.BuiltInDocumentProperties["Title"];
            titleProperty.Value = "Sample Workbook";
            
            // Visualizza le proprietà modificate
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Title: " + workbook.BuiltInDocumentProperties["Title"].Value);
        }
    }
}
```

### Vedi anche

* class [BuiltInDocumentPropertyCollection](../../../aspose.cells.properties/builtindocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


