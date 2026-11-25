---
title: "Name.FullText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Name. Ottiene il testo completo del nome dell'oggetto con l'impostazione di ambito"
type: docs
url: /it/net/aspose.cells/name/fulltext/
---
## Name.FullText property

Ottiene il testo completo del nome dell'oggetto con l'impostazione di ambito.

```csharp
public string FullText { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyFullTextDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea alcuni intervalli denominati
            worksheet.Cells["A1"].PutValue("Test Value");
            worksheet.Cells.CreateRange("A1", "B5").Name = "TestRange1";
            worksheet.Cells.CreateRange("C1", "D5").Name = "TestRange2";
            
            // Ottieni la collezione di nomi
            NameCollection names = workbook.Worksheets.Names;
            
            // Trova un nome per il suo FullText
            string reference = "=Sheet1!$A$1:$B$5";
            Name foundName = FindNameByFullText(names, reference);
            
            // Restituisci i risultati
            if (foundName != null)
            {
                Console.WriteLine("Found name: " + foundName.Text);
                Console.WriteLine("FullText: " + foundName.FullText);
            }
            else
            {
                Console.WriteLine("Name not found");
            }
        }
        
        public static Name FindNameByFullText(NameCollection names, string reference)
        {
            if (reference.IndexOf('=') == 0)
            {
                reference = reference.Substring(1);
            }
            foreach (Name nm in names)
            {
                if (nm.FullText.Equals(reference))
                {
                    return nm;
                }
            }
            return null;
        }
    }
}
```

### Vedi anche

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


