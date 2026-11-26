---
title: "Name.IsReferred"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Name. Указывает, используется ли это имя в других формулах"
type: docs
url: /ru/net/aspose.cells/name/isreferred/
---
## Name.IsReferred property

Указывает, используется ли это имя в других формулах.

```csharp
public bool IsReferred { get; }
```

### Примеры

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
            
            // Добавить имена
            Name n1 = nc[nc.Add("TestName1")];
            n1.RefersTo = "=Sheet1!F10:G15";

            Name n2 = nc[nc.Add("TestName2")];
            n2.RefersTo = "=Sheet1!H10:I15";

            // Добавить имена, ограниченные листом
            Name n3 = nc[nc.Add("Sheet1!TestName1")];
            n3.RefersTo = "=Sheet1!F20:G25";

            Name n4 = nc[nc.Add("Sheet1!TestName2")];
            n4.RefersTo = "=Sheet1!H20:I25";

            // Создать формулы, которые ссылаются на имена
            wb.Worksheets.Add();
            wb.Worksheets[1].Cells[0, 0].Formula = "=SUM(TestName2)";
            wb.Worksheets[0].Cells[0, 1].Formula = "=SUM(Sheet1!TestName2)";

            // Продемонстрировать свойство IsReferred
            Console.WriteLine($"TestName1.IsReferred: {n1.IsReferred}"); // False
            Console.WriteLine($"Sheet1!TestName1.IsReferred: {n3.IsReferred}"); // False
            Console.WriteLine($"TestName2.IsReferred: {n2.IsReferred}"); // True
            Console.WriteLine($"Sheet1!TestName2.IsReferred: {n4.IsReferred}"); // True
        }
    }
}
```

### См. также

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


