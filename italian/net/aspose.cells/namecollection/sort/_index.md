---
title: "NameCollection.Sort"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo NameCollection. Ordina i nomi definiti"
type: docs
url: /it/net/aspose.cells/namecollection/sort/
---
## NameCollection.Sort method

Ordina i nomi definiti.

```csharp
public void Sort()
```

### Osservazioni

Se crei un gran numero di intervalli denominati nel file Excel, chiama questo metodo dopo che tutti gli intervalli denominati sono stati creati e prima di salvare

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodSortDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni la NameCollection dalla cartella di lavoro
            NameCollection names = workbook.Worksheets.Names;
            
            // Aggiungi alcuni intervalli denominati per dimostrare l'ordinamento
            names.Add("RangeC");
            names.Add("RangeA");
            names.Add("RangeB");
            
            try
            {
                // Visualizza i nomi prima dell'ordinamento
                Console.WriteLine("Names before sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
                
                // Chiama il metodo Sort
                names.Sort();
                
                // Visualizza i nomi dopo l'ordinamento
                Console.WriteLine("\nNames after sorting:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Sort method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("NameCollectionSortDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


