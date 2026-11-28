---
title: "Workbook.Combine"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Başka bir Workbook nesnesini birleştirir"
type: docs
url: /tr/net/aspose.cells/workbook/combine/
---
## Workbook.Combine method

Başka bir Workbook nesnesiyle birleştirir.

```csharp
public void Combine(Workbook secondWorkbook)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| secondWorkbook | Çalışma Kitabı | Başka bir Workbook nesnesi. |

### Açıklamalar

Excel, ODS, CSV ve diğer dosyaları tek bir dosyada birleştirin.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCombineWithWorkbookDemo
    {
        public static void Run()
        {
            // Kaynak workbook oluşturun
            Workbook sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets[0].Cells["A1"].PutValue("Source Data");

            // Hedef çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook(FileFormatType.Xlsx);
            destWorkbook.Worksheets[0].Cells["B2"].PutValue("Destination Data");

            // Workbooks'ı birleştirin
            destWorkbook.Combine(sourceWorkbook);

            // Birleştirilen workbook'ı kaydedin
            destWorkbook.Save("CombinedWorkbook.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


