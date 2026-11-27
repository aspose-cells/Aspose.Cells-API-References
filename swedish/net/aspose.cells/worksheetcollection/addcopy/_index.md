---
title: "WorksheetCollection.AddCopy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorksheetCollection-metod. Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/addcopy/
---
## AddCopy(string) {#addcopy_1}

Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad.

```csharp
public int AddCopy(string sheetName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetName | String | Namn på källkalkylbladet. |

### Returvärde

[`Worksheet`](../../worksheet/) object index.

### Undantag

| undantag | villkor |
| --- | --- |
| [CellsException](../../cellsexception/) | Anger ett ogiltigt kalkylbladsnamn. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad med namnet "Original" i arbetsboken
            Worksheet originalSheet = workbook.Worksheets.Add("Original");
            
            // Lägg till lite data i det ursprungliga kalkylbladet
            originalSheet.Cells["A1"].PutValue("This is the original sheet");
            
            // Skapa en kopia av kalkylbladet "Original"
            int copiedIndex = workbook.Worksheets.AddCopy("Original");
            Worksheet copiedSheet = workbook.Worksheets[copiedIndex];
            copiedSheet.Name = "CopiedSheet";
            
            // Modifiera det kopierade bladet för att visa att det är en separat kopia
            copiedSheet.Cells["A1"].PutValue("This is the copied sheet");
            
            // Spara arbetsboken
            workbook.Save("WorksheetCopyDemo.xlsx");
            
            Console.WriteLine("Worksheet copied successfully. Output file: WorksheetCopyDemo.xlsx");
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(int) {#addcopy}

Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad.

```csharp
public int AddCopy(int sheetIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | Int32 | Index för källkalkylbladet. |

### Returvärde

[`Worksheet`](../../worksheet/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till första kalkylbladet och lägg till lite data
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Worksheet");
            
            // Lägg till en kopia av det första kalkylbladet
            workbook.Worksheets.AddCopy(0);
            
            // Verifiera att kopian skapades
            Worksheet copiedWorksheet = workbook.Worksheets[1];
            copiedWorksheet.Cells["A1"].PutValue("Copied Worksheet");
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Worksheet[], string[]) {#addcopy_2}

Kopiera en grupp kalkylblad.

```csharp
public void AddCopy(Worksheet[] source, string[] destSheetNames)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | Worksheet[] | Källkalkylbladen. |
| destSheetNames | String[] | Namnen på de kopierade bladen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodAddCopyWithWorksheetStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till några exempel på kalkylblad
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Fyll i lite data i kalkylbladen
            workbook.Worksheets["Sheet2"].Cells["A1"].PutValue("Original Sheet1 Data");
            workbook.Worksheets["Sheet3"].Cells["A1"].PutValue("Original Sheet2 Data");

            // Förbered arrayen med källkalkylblad
            Worksheet[] sourceSheets = new Worksheet[]
            {
                workbook.Worksheets["Sheet2"],
                workbook.Worksheets["Sheet3"]
            };

            // Förbered arrayen med destinationsbladnamn
            string[] destSheetNames = new string[]
            {
                "CopyOfSheet2",
                "CopyOfSheet3"
            };

            try
            {
                // Anropa AddCopy-metoden med parametrarna (Worksheet[], String[])
                workbook.Worksheets.AddCopy(sourceSheets, destSheetNames);
                
                Console.WriteLine("AddCopy method executed successfully with parameters (Worksheet[], String[])");
                
                // Verifiera att kopiorna skapades
                Console.WriteLine($"Total worksheets after copy: {workbook.Worksheets.Count}");
                foreach (Worksheet sheet in workbook.Worksheets)
                {
                    Console.WriteLine($"Worksheet name: {sheet.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddCopy method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("WorksheetCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


