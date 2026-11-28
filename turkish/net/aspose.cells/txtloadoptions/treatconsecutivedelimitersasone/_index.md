---
title: "TxtLoadOptions.TreatConsecutiveDelimitersAsOne"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TxtLoadOptions özelliği. Ardışık ayırıcıların tek olarak ele alınması gerekir"
type: docs
url: /tr/net/aspose.cells/txtloadoptions/treatconsecutivedelimitersasone/
---
## TxtLoadOptions.TreatConsecutiveDelimitersAsOne property

Ardışık sınırlayıcıların tek olarak ele alınıp alınmayacağı.

```csharp
public bool TreatConsecutiveDelimitersAsOne { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyTreatConsecutiveDelimitersAsOneDemo
    {
        public static void Run()
        {
            // Örnek 1: Varsayılan davranış (TreatConsecutiveDelimitersAsOne = false)
            TxtLoadOptions options1 = new TxtLoadOptions(LoadFormat.Csv);
            options1.TreatConsecutiveDelimitersAsOne = false;
            
            string csvData1 = "1,\"abc\",3,'def'\n\"\"\"g'hi\",,,\n'jkl\"',,,12";
            Workbook workbook1 = new Workbook(new MemoryStream(Encoding.UTF8.GetBytes(csvData1)), options1);
            Cells cells1 = workbook1.Worksheets[0].Cells;
            
            Console.WriteLine("Default behavior (TreatConsecutiveDelimitersAsOne = false):");
            Console.WriteLine("B1 value: " + cells1["B1"].StringValue); // abc
            Console.WriteLine("D1 value: " + cells1["D1"].StringValue); // 'def'
            Console.WriteLine("B3 is null: " + (cells1["B3"].Type == CellValueType.IsNull)); // True
            Console.WriteLine("D3 value: " + cells1["D3"].IntValue); // 12

            // Örnek 2: TreatConsecutiveDelimitersAsOne = true
            TxtLoadOptions options2 = new TxtLoadOptions(LoadFormat.Csv);
            options2.TreatConsecutiveDelimitersAsOne = true;
            
            string csvData2 = "1,\"abc\",3,'def'\n\"\"\"g'hi\",,,\n'jkl\"',,,12";
            Workbook workbook2 = new Workbook(new MemoryStream(Encoding.UTF8.GetBytes(csvData2)), options2);
            Cells cells2 = workbook2.Worksheets[0].Cells;
            
            Console.WriteLine("\nWith TreatConsecutiveDelimitersAsOne = true:");
            Console.WriteLine("D3 is null: " + (cells2["D3"].Type == CellValueType.IsNull)); // True
            Console.WriteLine("B3 value: " + cells2["B3"].IntValue); // 12

            // Örnek 3: Boşluk ayırıcı olarak kullanma
            TxtLoadOptions options3 = new TxtLoadOptions(LoadFormat.Csv);
            options3.Separator = ' ';
            options3.TreatConsecutiveDelimitersAsOne = true;
            
            string csvData3 = "1 \"abc\" 3 'def'\n\"\"\"g'hi\"   \n'jkl\"'   12";
            Workbook workbook3 = new Workbook(new MemoryStream(Encoding.UTF8.GetBytes(csvData3)), options3);
            Cells cells3 = workbook3.Worksheets[0].Cells;
            
            Console.WriteLine("\nWith space separator and TreatConsecutiveDelimitersAsOne = true:");
            Console.WriteLine("B1 value: " + cells3["B1"].StringValue); // abc
            Console.WriteLine("B3 value: " + cells3["B3"].IntValue); // 12
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


