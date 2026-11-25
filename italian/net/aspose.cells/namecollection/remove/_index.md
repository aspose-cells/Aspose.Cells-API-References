---
title: "NameCollection.Remove"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo NameCollection. Rimuovi un array di nomi"
type: docs
url: /it/net/aspose.cells/namecollection/remove/
---
## Remove(string[]) {#remove_1}

Rimuovi un array di nomi

```csharp
public void Remove(string[] names)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nomi | String[] | Il testo dei nomi. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodRemoveWithStringArrayDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ottieni la NameCollection dalla cartella di lavoro
            NameCollection names = workbook.Worksheets.Names;
            
            // Aggiungi alcuni intervalli denominati per dimostrare la rimozione
            names.Add("TestRange1");
            names.Add("TestRange2");
            names.Add("TestRange3");
            
            // Prepara l'array di nomi da rimuovere
            string[] namesToRemove = new string[] { "TestRange1", "TestRange3" };

            try
            {
                // Chiama il metodo Remove con parametro String[]
                names.Remove(namesToRemove);
                
                Console.WriteLine("Names removed successfully:");
                foreach (string name in namesToRemove)
                {
                    Console.WriteLine(name);
                }
                
                // Mostra i nomi rimanenti
                Console.WriteLine("\nRemaining names in the collection:");
                foreach (Name name in names)
                {
                    Console.WriteLine(name.Text);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("NameCollectionRemoveDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove}

Rimuovi il nome.

```csharp
public void Remove(string text)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | String | Il testo del nome. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi un intervallo denominato
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1", "B10");
            range.Name = "TestRange";
            
            // Visualizza il conteggio prima della rimozione
            Console.WriteLine("Named ranges count before removal: " + workbook.Worksheets.Names.Count);
            
            // Rimuovi l'intervallo denominato
            workbook.Worksheets.Names.Remove("TestRange");
            
            // Visualizza il conteggio dopo la rimozione
            Console.WriteLine("Named ranges count after removal: " + workbook.Worksheets.Names.Count);
        }
    }
}
```

### Vedi anche

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


