---
title: "WorksheetCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. Belirtilen indeksteki Worksheet öğesini alır"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/item/
---
## WorksheetCollection indexer (1 of 2)

Belirtilen indeksteki [`Worksheet`](../../worksheet/) öğesini alır.

```csharp
public Worksheet this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Hücreye erişmek için Item özelliğini kullanma
            Cell cell = cells[0, 0];
            cell.Formula = "=SUM(1, 2, 3)";
            
            workbook.CalculateFormula();
            Console.WriteLine("Cell value: " + cell.IntValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorksheetCollection indexer (2 of 2)

Belirtilen adla [`Worksheet`](../../worksheet/) öğesini alır.

```csharp
public Worksheet this[string sheetName] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| sheetName | Çalışma sayfası adı |

### Dönüş Değeri

Belirtilen ada sahip öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İndeks ve ad ile Item özelliğini kullanarak çalışma sayfalarına erişin
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            
            // Item özelliğini kullanarak adıyla çalışma sayfasına erişin
            Worksheet accessedSheet = workbook.Worksheets["FirstSheet"];
            
            // Çalışma sayfası erişimini göstermek için veri ekleyin
            Cells cells = accessedSheet.Cells;
            cells["A1"].PutValue("Worksheet accessed successfully!");
            cells["A2"].PutValue(DateTime.Now.ToString());
            
            // İkinci sayfaya bir sütun ekleyin
            workbook.Worksheets["SecondSheet"].Cells.InsertColumn(1);
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetCollectionItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


