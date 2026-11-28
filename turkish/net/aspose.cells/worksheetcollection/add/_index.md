---
title: "WorksheetCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Bir çalışma sayfasını koleksiyona ekler"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/add/
---
## Add(SheetType) {#add_2}

Koleksiyona bir çalışma sayfası ekler.

```csharp
public int Add(SheetType type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | SheetType | Worksheet türü. |

### Dönüş Değeri

[`Worksheet`](../../worksheet/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddWithSheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // SheetType parametresini kullanarak yeni bir grafik sayfası ekleyin
            workbook.Worksheets.Add(SheetType.Chart);
            
            // İlk çalışma sayfasına veri ekleyin
            Cells cells = workbook.Worksheets[0].Cells;
            cells["C2"].PutValue(5000);
            cells["C3"].PutValue(3000);
            cells["C4"].PutValue(4000);
            cells["C5"].PutValue(5000);
            cells["C6"].PutValue(6000);
            
            // Grafik sayfasında grafik oluşturun
            Aspose.Cells.Charts.ChartCollection charts = workbook.Worksheets[1].Charts;
            int chartIndex = charts.Add(Aspose.Cells.Charts.ChartType.Column, 10, 10, 20, 20);
            Aspose.Cells.Charts.Chart chart = charts[chartIndex];
            chart.NSeries.Add("Sheet1!C2:C6", true);
            
            // Çalışma kitabını kaydedin (isteğe bağlı)
            // workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add() {#add_1}

Koleksiyona bir çalışma sayfası ekler.

```csharp
public int Add()
```

### Dönüş Değeri

[`Worksheet`](../../worksheet/) object index.

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add}

Koleksiyona bir çalışma sayfası ekler.

```csharp
public Worksheet Add(string sheetName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | String | Çalışma sayfası adı |

### Dönüş Değeri

[`Worksheet`](../../worksheet/) object.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets.Add("NewSheet");
            
            // Yeni çalışma sayfasına veri ekleyin
            worksheet.Cells["A1"].PutValue("Worksheet added successfully!");
            
            // Çalışma kitabını kaydedin
            wb.Save("WorksheetCollectionMethodAddWithStringDemo_output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


