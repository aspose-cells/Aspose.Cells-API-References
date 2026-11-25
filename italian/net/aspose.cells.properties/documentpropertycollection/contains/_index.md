---
title: "DocumentPropertyCollection.Contains"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DocumentPropertyCollection. Restituisce true se una proprietà con il nome specificato esiste nella collezione"
type: docs
url: /it/net/aspose.cells.properties/documentpropertycollection/contains/
---
## DocumentPropertyCollection.Contains method

Restituisce true se una proprietà con il nome specificato esiste nella raccolta.

```csharp
public bool Contains(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della proprietà, senza distinzione tra maiuscole e minuscole. |

### Valore di ritorno

True se la proprietà esiste nella collezione; false altrimenti.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionMethodContainsWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Verifica se la proprietà "RevisionNumber" esiste nelle proprietà del documento predefinite
            bool containsRevision = workbook.BuiltInDocumentProperties.Contains("RevisionNumber");
            Console.WriteLine("Contains 'RevisionNumber': " + containsRevision);
            
            // Aggiungi una proprietà personalizzata e verifica la sua esistenza
            workbook.CustomDocumentProperties.Add("CustomProperty", "Test Value");
            bool containsCustom = workbook.CustomDocumentProperties.Contains("CustomProperty");
            Console.WriteLine("Contains 'CustomProperty': " + containsCustom);
        }
    }
}
```

### Vedi anche

* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


