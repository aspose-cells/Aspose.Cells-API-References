---
title: "Name.IsReferred"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Name özelliği. Bu adın diğer formüller tarafından başvurulup başvurulmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/name/isreferred/
---
## Name.IsReferred property

Bu adın diğer formüller tarafından referans alınıp alınmadığını gösterir.

```csharp
public bool IsReferred { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyIsReferredDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            NameCollection nc = wb.Worksheets.Names;
            
            // Adlar ekle
            Name n1 = nc[nc.Add("TestName1")];
            n1.RefersTo = "=Sheet1!F10:G15";

            Name n2 = nc[nc.Add("TestName2")];
            n2.RefersTo = "=Sheet1!H10:I15";

            // Çalışma sayfası kapsamlı adlar ekle
            Name n3 = nc[nc.Add("Sheet1!TestName1")];
            n3.RefersTo = "=Sheet1!F20:G25";

            Name n4 = nc[nc.Add("Sheet1!TestName2")];
            n4.RefersTo = "=Sheet1!H20:I25";

            // Adlara başvuran formüller oluştur
            wb.Worksheets.Add();
            wb.Worksheets[1].Cells[0, 0].Formula = "=SUM(TestName2)";
            wb.Worksheets[0].Cells[0, 1].Formula = "=SUM(Sheet1!TestName2)";

            // IsReferred özelliğini göster
            Console.WriteLine($"TestName1.IsReferred: {n1.IsReferred}"); // False
            Console.WriteLine($"Sheet1!TestName1.IsReferred: {n3.IsReferred}"); // False
            Console.WriteLine($"TestName2.IsReferred: {n2.IsReferred}"); // True
            Console.WriteLine($"Sheet1!TestName2.IsReferred: {n4.IsReferred}"); // True
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


