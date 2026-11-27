---
title: "WorksheetCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Tar bort elementet med ett angivet namn"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Tar bort elementet med ett angivet namn.

```csharp
public void RemoveAt(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på elementet som ska tas bort. |

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Lägg till några arbetsblad
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");
            
            // Lägg till ett namngivet område (fast)
            int nameIndex = wb.Worksheets.Names.Add("testname");
            wb.Worksheets.Names[nameIndex].RefersTo = "=[Book1.xlsx]Sheet1!$A1";
            
            // Demonstrera RemoveAt med strängparameter
            Console.WriteLine($"Before removal - Worksheet count: {wb.Worksheets.Count}");
            wb.Worksheets.RemoveAt("Sheet1");
            Console.WriteLine($"After removal - Worksheet count: {wb.Worksheets.Count}");
            
            // Spara arbetsboken
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
            }
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int) {#removeat}

Tar bort elementet vid ett angivet index.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Indexvärdet för elementet som ska tas bort. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Lägg till några arbetsblad
            wb.Worksheets.Add("Sheet1");
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");

            // Visa ursprungligt antal arbetsblad
            Console.WriteLine($"Original worksheet count: {wb.Worksheets.Count}");

            // Ta bort arbetsbladet på index 1 (andra arbetsbladet)
            wb.Worksheets.RemoveAt(1);

            // Visa uppdaterat antal arbetsblad
            Console.WriteLine($"After removal, worksheet count: {wb.Worksheets.Count}");

            // Spara arbetsboken
            wb.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


