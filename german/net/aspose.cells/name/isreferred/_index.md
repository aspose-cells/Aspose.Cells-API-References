---
title: "Name.IsReferred"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Name-Eigenschaft. Gibt an, ob dieser Name von anderen Formeln referenziert wird"
type: docs
url: /de/net/aspose.cells/name/isreferred/
---
## Name.IsReferred property

Gibt an, ob dieser Name von anderen Formeln referenziert wird.

```csharp
public bool IsReferred { get; }
```

### Beispiele

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
            
            // Namen hinzufügen
            Name n1 = nc[nc.Add("TestName1")];
            n1.RefersTo = "=Sheet1!F10:G15";

            Name n2 = nc[nc.Add("TestName2")];
            n2.RefersTo = "=Sheet1!H10:I15";

            // Arbeitsblattbezogene Namen hinzufügen
            Name n3 = nc[nc.Add("Sheet1!TestName1")];
            n3.RefersTo = "=Sheet1!F20:G25";

            Name n4 = nc[nc.Add("Sheet1!TestName2")];
            n4.RefersTo = "=Sheet1!H20:I25";

            // Formeln erstellen, die die Namen referenzieren
            wb.Worksheets.Add();
            wb.Worksheets[1].Cells[0, 0].Formula = "=SUM(TestName2)";
            wb.Worksheets[0].Cells[0, 1].Formula = "=SUM(Sheet1!TestName2)";

            // Demonstration der IsReferred-Eigenschaft
            Console.WriteLine($"TestName1.IsReferred: {n1.IsReferred}"); // False
            Console.WriteLine($"Sheet1!TestName1.IsReferred: {n3.IsReferred}"); // False
            Console.WriteLine($"TestName2.IsReferred: {n2.IsReferred}"); // True
            Console.WriteLine($"Sheet1!TestName2.IsReferred: {n4.IsReferred}"); // True
        }
    }
}
```

### Siehe auch

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


