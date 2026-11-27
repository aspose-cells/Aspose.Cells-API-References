---
title: "Klassen ProtectedRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ProtectedRange-klass. Ett specificerat område som får redigeras när bladskyddet är PÅ"
type: docs
url: /sv/net/aspose.cells/protectedrange/
---
## ProtectedRange class

Ett specificerat område som får redigeras när bladskyddet är AKTIVT.

```csharp
public class ProtectedRange
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CellArea](../../aspose.cells/protectedrange/cellarea/) { get; } | Hämtar [`CellArea`](./cellarea/)‑objektet som representerar det cellområde som ska skyddas. |
| [IsProtectedWithPassword](../../aspose.cells/protectedrange/isprotectedwithpassword/) { get; } | Anger om kalkylbladen är skyddade med lösenord. |
| [Name](../../aspose.cells/protectedrange/name/) { get; set; } | Hämtar områdestiteln. Den används som en beskrivning, inte som en namngiven områdesdefinition. |
| [Password](../../aspose.cells/protectedrange/password/) { get; set; } | Representerar lösenordet för att skydda området. |
| [SecurityDescriptor](../../aspose.cells/protectedrange/securitydescriptor/) { get; set; } | Säkerhetsbeskrivningen definierar användarkonton som kan redigera detta område utan att ange ett lösenord för att komma åt området. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddArea](../../aspose.cells/protectedrange/addarea/)(int, int, int, int) | Lägger till ett refererat område till detta |
| [GetAreas](../../aspose.cells/protectedrange/getareas/)() | Hämtar alla refererade områden. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassProtectedRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta samlingen av skyddade områden
            ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
            
            // Lägg till ett nytt skyddat område (A1:J10)
            int index = protectedRanges.Add("MyProtectedRange", 0, 0, 10, 10);
            
            // Hämta det skyddade området
            ProtectedRange protectedRange = protectedRanges[index];
            
            // Ställ in säkerhetsbeskrivning
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            protectedRange.SecurityDescriptor = securityDescriptor;
            
            // Spara arbetsboken
            workbook.Save("ProtectedRangeDemo.xlsx");
            
            Console.WriteLine("Protected range demo completed successfully.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


