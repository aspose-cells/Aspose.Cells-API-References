---
title: "Arayüz ICellsDataTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ICellsDataTable arayüzü. Veri tablosunu temsil eder"
type: docs
url: /tr/net/aspose.cells/icellsdatatable/
---
## ICellsDataTable interface

Veri tablosunu temsil eder.

```csharp
public interface ICellsDataTable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Columns](../../aspose.cells/icellsdatatable/columns/) { get; } | Sütunların adını alır. |
| [Count](../../aspose.cells/icellsdatatable/count/) { get; } | Kayıtların sayısını alır. Bilinmeyen kayıt sayısı için -1. |
| [Item](../../aspose.cells/icellsdatatable/item/) { get; } | İndeks ile belirtilen sütunda depolanan veriyi alır. (2 indeksleyici) |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [BeforeFirst](../../aspose.cells/icellsdatatable/beforefirst/)() | İmleci bu nesnenin başına, ilk satırın hemen önüne taşı. |
| [Next](../../aspose.cells/icellsdatatable/next/)() | İmleci mevcut konumundan bir satır aşağı hareket ettirir. |

### Örnekler

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassICellsDataTableDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();

            ArrayList dataLists = new ArrayList();
            ArrayList list1 = new ArrayList();
            list1.AddRange(new object[] { "Name", "Age", "Gender" });
            ArrayList list2 = new ArrayList();
            list2.AddRange(new object[] { "Alice", 30, "Female" });
            ArrayList list3 = new ArrayList();
            list3.AddRange(new object[] { "Bob", 25, "Male" });
            ArrayList list4 = new ArrayList();
            list4.AddRange(new object[] { "Charlie", 35, "Male" });
            dataLists.Add(list1);
            dataLists.Add(list2);
            dataLists.Add(list3);
            dataLists.Add(list4);

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
            
            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            Console.WriteLine("First worksheet A2 value: " + wb.Worksheets[0].Cells["A2"].StringValue);

            wb.Worksheets.Add();
            wb.Worksheets[1].Cells.ImportArrayList(dataLists, 0, 0, true);
            Console.WriteLine("Second worksheet A3 value: " + wb.Worksheets[1].Cells["A3"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


