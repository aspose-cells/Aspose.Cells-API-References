---
title: "VbaModuleCollection.Remove"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VbaModuleCollection-metoden. Tar bort modul för ett kalkylblad"
type: docs
url: /sv/net/aspose.cells.vba/vbamodulecollection/remove/
---
## Remove(Worksheet) {#remove}

Tar bort modul för ett kalkylblad.

```csharp
public void Remove(Worksheet sheet)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| blad | Arbetsblad | Arbetsbladet |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleCollectionMethodRemoveWithWorksheetDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en VBA-modul till kalkylbladet
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Hämta VBA-modulsamlingen
            VbaModuleCollection modules = workbook.VbaProject.Modules;
            
            try
            {
                // Anropa Remove-metoden med kalkylbladsparametern
                modules.Remove(worksheet);
                
                Console.WriteLine("VBA module removed successfully for the specified worksheet.");
                
                // Verifiera att modulen togs bort
                if (modules.Count == 0)
                {
                    Console.WriteLine("No VBA modules remain in the collection.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("VbaModuleRemoveWithWorksheetDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove_1}

Ta bort modulen efter namn

```csharp
public void Remove(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String |  |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med makro
            Workbook workbook = new Workbook();
            
            // Få åtkomst till VBA-projekt
            VbaProject vbaProject = workbook.VbaProject;
            
            // Lägg till en ny modul
            int index = vbaProject.Modules.Add(VbaModuleType.Procedural, "TestModule");
            
            // Lägg till kod i modulen
            vbaProject.Modules[index].Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";
            
            // Spara arbetsboken
            workbook.Save("output_with_module.xlsm");
            
            // Ta bort modulen efter namn
            vbaProject.Modules.Remove("TestModule");
            
            // Spara arbetsboken efter borttagning
            workbook.Save("output_after_removal.xlsm");
        }
    }
}
```

### Se även

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


