---
title: "Name.R1C1RefersTo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Name özelliği. Name'in bir R1C1 referansını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/name/r1c1refersto/
---
## Name.R1C1RefersTo property

[`Name`](../) öğesinin bir R1C1 referansını alır veya ayarlar.

```csharp
public string R1C1RefersTo { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyR1C1RefersToDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Adlar koleksiyonuna yeni bir ad ekleyin
            int nameIndex = workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names[nameIndex];
            
            // Ad için R1C1 referansını ayarla
            name.R1C1RefersTo = "'Sheet1'!R3C1:R9C4";
            
            // Referansın doğru ayarlandığını doğrula
            Console.WriteLine("Name refers to: " + name.RefersTo);
            
            // Çalışma kitabını kaydedin
            workbook.Save("NamePropertyR1C1RefersToDemo_Output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


