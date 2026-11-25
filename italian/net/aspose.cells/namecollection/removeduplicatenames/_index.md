---
title: "NameCollection.RemoveDuplicateNames"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo NameCollection. Rimuovi i nomi definiti duplicati"
type: docs
url: /it/net/aspose.cells/namecollection/removeduplicatenames/
---
## NameCollection.RemoveDuplicateNames method

Rimuovi i nomi definiti duplicati

```csharp
public void RemoveDuplicateNames()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveDuplicateNamesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni intervalli denominati con nomi duplicati
            worksheet.Cells["A1"].PutValue("Test Value 1");
            worksheet.Cells["B1"].PutValue("Test Value 2");
            
            // Crea intervalli denominati duplicati usando la corretta firma del metodo Add
            int index1 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index1].RefersTo = "=Sheet1!$A$1";
            
            int index2 = workbook.Worksheets.Names.Add("DuplicateName");
            workbook.Worksheets.Names[index2].RefersTo = "=Sheet1!$B$1";
            
            // Mostra il conteggio prima di rimuovere i duplicati
            Console.WriteLine($"Named ranges count before removal: {workbook.Worksheets.Names.Count}");
            
            // Rimuovi i nomi duplicati
            workbook.Worksheets.Names.RemoveDuplicateNames();
            
            // Mostra il conteggio dopo aver rimosso i duplicati
            Console.WriteLine($"Named ranges count after removal: {workbook.Worksheets.Names.Count}");
        }
    }
}
```

### Vedi anche

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


