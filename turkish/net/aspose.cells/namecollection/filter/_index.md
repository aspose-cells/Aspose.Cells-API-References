---
title: "NameCollection.Filter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "NameCollection yöntemi. Kapsama göre tanımlı tüm adları alır"
type: docs
url: /tr/net/aspose.cells/namecollection/filter/
---
## NameCollection.Filter method

Kapsama göre tüm tanımlı adları alır.

```csharp
public Name[] Filter(NameScopeType type, int sheetIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | NameScopeType | Kapsam türü. |
| sheetIndex | Int32 | Sayfa indeksi. Yalnızca kapsam türü Worksheet olduğunda etkili olur |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodFilterWithNameScopeTypeInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabına ve çalışma sayfalarına bazı adlar ekleyin
            workbook.Worksheets.Names.Add("GlobalName");
            Worksheet worksheet1 = workbook.Worksheets[0];
            workbook.Worksheets.Names.Add("Sheet1Name");
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Names.Add("Sheet2Name");

            // Adları kapsam türüne ve sayfa indeksine göre filtreleyin
            Name[] workbookScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1);
            Name[] worksheetScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1);
            Name[] sheet1Names = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 0);

            // Sonuçları çıktı olarak ver
            Console.WriteLine($"Workbook-scoped names count: {workbookScopeNames.Length}");
            Console.WriteLine($"Worksheet-scoped names count: {worksheetScopeNames.Length}");
            Console.WriteLine($"Sheet1 names count: {sheet1Names.Length}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../../name/)
* enum [NameScopeType](../../namescopetype/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


