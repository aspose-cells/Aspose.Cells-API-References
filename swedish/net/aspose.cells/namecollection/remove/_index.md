---
title: "NameCollection.Remove"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NameCollection-metoden. Ta bort en array av namn"
type: docs
url: /sv/net/aspose.cells/namecollection/remove/
---
## Remove(string[]) {#remove_1}

Ta bort en array av namn

```csharp
public void Remove(string[] names)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String[] | Texten för namnen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionMethodRemoveWithStringArrayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta NameCollection från arbetsboken
            NameCollection names = workbook.Worksheets.Names;
            
            // Lägg till några namngivna områden för att demonstrera borttagning
            names.Add("TestRange1");
            names.Add("TestRange2");
            names.Add("TestRange3");
            
            // Förbered arrayen med namn som ska tas bort
            string[] namesToRemove = new string[] { "TestRange1", "TestRange3" };

            try
            {
                // Anropa Remove-metoden med String[]-parameter
                names.Remove(namesToRemove);
                
                Console.WriteLine("Names removed successfully:");
                foreach (string name in namesToRemove)
                {
                    Console.WriteLine(name);
                }
                
                // Visa återstående namn
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
            
            // Spara resultatet
            workbook.Save("NameCollectionRemoveDemo.xlsx");
        }
    }
}
```

### Se även

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove}

Ta bort namnet.

```csharp
public void Remove(string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | Namnetexten. |

### Exempel

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
            
            // Lägg till ett namngivet område
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1", "B10");
            range.Name = "TestRange";
            
            // Visa antalet före borttagning
            Console.WriteLine("Named ranges count before removal: " + workbook.Worksheets.Names.Count);
            
            // Ta bort det namngivna området
            workbook.Worksheets.Names.Remove("TestRange");
            
            // Visa antalet efter borttagning
            Console.WriteLine("Named ranges count after removal: " + workbook.Worksheets.Names.Count);
        }
    }
}
```

### Se även

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


