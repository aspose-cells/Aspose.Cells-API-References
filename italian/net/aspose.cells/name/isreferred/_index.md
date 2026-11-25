---
title: "Name.IsReferred"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Name. Indica se questo nome è riferito da altre formule"
type: docs
url: /it/net/aspose.cells/name/isreferred/
---
## Name.IsReferred property

Indica se questo nome è referenziato da altre formule.

```csharp
public bool IsReferred { get; }
```

### Esempi

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
            
            // Aggiungi nomi
            Name n1 = nc[nc.Add("TestName1")];
            n1.RefersTo = "=Sheet1!F10:G15";

            Name n2 = nc[nc.Add("TestName2")];
            n2.RefersTo = "=Sheet1!H10:I15";

            // Aggiungi nomi con ambito di foglio di lavoro
            Name n3 = nc[nc.Add("Sheet1!TestName1")];
            n3.RefersTo = "=Sheet1!F20:G25";

            Name n4 = nc[nc.Add("Sheet1!TestName2")];
            n4.RefersTo = "=Sheet1!H20:I25";

            // Crea formule che fanno riferimento ai nomi
            wb.Worksheets.Add();
            wb.Worksheets[1].Cells[0, 0].Formula = "=SUM(TestName2)";
            wb.Worksheets[0].Cells[0, 1].Formula = "=SUM(Sheet1!TestName2)";

            // Dimostra la proprietà IsReferred
            Console.WriteLine($"TestName1.IsReferred: {n1.IsReferred}"); // False
            Console.WriteLine($"Sheet1!TestName1.IsReferred: {n3.IsReferred}"); // False
            Console.WriteLine($"TestName2.IsReferred: {n2.IsReferred}"); // True
            Console.WriteLine($"Sheet1!TestName2.IsReferred: {n4.IsReferred}"); // True
        }
    }
}
```

### Vedi anche

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


