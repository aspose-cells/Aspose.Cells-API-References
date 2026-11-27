---
title: "ExternalLinkCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExternalLinkCollection‑metod. Tar bort den angivna externa länken från arbetsboken"
type: docs
url: /sv/net/aspose.cells/externallinkcollection/removeat/
---
## RemoveAt(int) {#removeat}

Tar bort den angivna externa länken från arbetsboken.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | indexet för den externa länken som ska tas bort. |

### Anmärkningar

När den externa länken tas bort kommer alla formler som refererar till den också att tas bort eftersom referenserna blir ogiltiga.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempel på externa länkar
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till några exempel på externa länkar
            worksheet.Cells["A1"].Formula = "='C:/ExternalFiles/File1.xlsx'!Sheet1!A1";
            worksheet.Cells["A2"].Formula = "='C:/ExternalFiles/File2.xlsx'!Sheet1!A1";
            worksheet.Cells["A3"].Formula = "='C:/ImportantFiles/File3.xlsx'!Sheet1!A1";

            // Hämta samling av externa länkar
            ExternalLinkCollection elc = workbook.Worksheets.ExternalLinks;
            Console.WriteLine("Initial external links count: " + elc.Count);

            // Ta bort externa länkar som inte innehåller "ImportantFiles" i deras sökväg
            for (int i = elc.Count - 1; i >= 0; i--)
            {
                if (!elc[i].DataSource.Contains("ImportantFiles"))
                {
                    elc.RemoveAt(i);
                }
            }

            Console.WriteLine("Remaining external links count: " + elc.Count);
            Console.WriteLine("Remaining external link path: " + elc[0].DataSource);
        }
    }
}
```

### Se även

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_1}

Tar bort den angivna externa länken från arbetsboken.

```csharp
public void RemoveAt(int index, bool updateReferencesAsLocal)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | indexet för den externa länken som ska tas bort. |
| updateReferencesAsLocal | Boolean | Om alla referenser för den angivna externa länken ska uppdateras till en referens till den aktuella arbetsboken själv. Kontrollera [`Clear`](../clear/) för att få mer detaljer om denna parameter. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodRemoveAtWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook wb = new Workbook();
            
            // Lägg till några externa länkar
            ExternalLinkCollection elc = wb.Worksheets.ExternalLinks;
            elc.Add("externallink1.xlam", new string[] { "externallink1.xlam" });
            elc.Add("externallink2.xlam", new string[] { "externallink2.xlam" });
            elc.Add("externallink3.xlam", new string[] { "externallink3.xlam" });
            elc.Add("externallink4.xlam", new string[] { "externallink4.xlam" });

            // Lägg till några formler som refererar till dessa externa länkar
            Worksheet ws = wb.Worksheets[0];
            for (int i = 0; i < 4; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    ws.Cells[j, i].Formula = $"=externallink{i+1}.xlam!customfunc{j+1}()";
                }
            }

            Console.WriteLine($"Initial external links count: {elc.Count}");
            Console.WriteLine("Formulas before removal:");
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {ws.Cells[0, i].Formula}");
            }

            // Ta bort vid index 1 med updateReferences=true
            elc.RemoveAt(1, true);
            
            Console.WriteLine($"\nAfter removing at index 1 (updateReferences=true):");
            Console.WriteLine($"External links count: {elc.Count}");
            Console.WriteLine("Updated formulas:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {ws.Cells[0, i].Formula}");
            }

            // Ta bort vid index 0 med updateReferences=false
            elc.RemoveAt(0, false);
            
            Console.WriteLine($"\nAfter removing at index 0 (updateReferences=false):");
            Console.WriteLine($"External links count: {elc.Count}");
            Console.WriteLine("Formulas (should be cleared where references were removed):");
            for (int i = 0; i < 2; i++)
            {
                Console.WriteLine($"Cell A{i+1}: Has formula? {ws.Cells[0, i].IsFormula}");
            }
        }
    }
}
```

### Se även

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


