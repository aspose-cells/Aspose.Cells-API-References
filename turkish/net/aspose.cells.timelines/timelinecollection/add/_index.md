---
title: "TimelineCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TimelineCollection yöntemi. Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle"
type: docs
url: /tr/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

PivotTable'ı veri kaynağı olarak kullanarak yeni bir Timeline ekle.

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| satır | Int32 | Timeline aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | Int32 | Timeline aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| baseFieldName | String | PivotTable.BaseFields içindeki PivotField'ın adı |

### Dönüş Değeri

Yeni eklenen Timeline dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri oluştur
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 1, 3);
            cells["C4"].Value = 200;

            // Özet tablo oluştur
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Column, 1);
            pivot.AddFieldToArea(PivotFieldType.Data, 2);

            // Pivot tabloya bağlanan timeline ekle
            sheet.Timelines.Add(pivot, 10, 5, "Date");
            
            // Çalışma kitabını kaydet
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

PivotTable'ı veri kaynağı olarak kullanarak yeni bir Timeline ekle.

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| destCellName | String | Timeline aralığının sol üst köşesindeki hücre adı. |
| baseFieldName | String | PivotTable.BaseFields içindeki PivotField'ın adı |

### Dönüş Değeri

Yeni eklenen Timeline dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            
            // Pivot tablo ekle
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "C1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Pivot tabloya bağlanan timeline ekle
            sheet.Timelines.Add(pivot, "E1", "Date");
            
            // Çalışma kitabını kaydedin
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

PivotTable'ı veri kaynağı olarak kullanarak yeni bir Timeline ekle.

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| satır | Int32 | Timeline aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | Int32 | Timeline aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| baseFieldIndex | Int32 | PivotTable.BaseFields içindeki PivotField'ın dizini |

### Dönüş Değeri

Yeni eklenen Timeline dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri oluştur
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Pivot tablo ekle
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // timeline denetimi ekle
            sheet.Timelines.Add(pivot, 15, 5, 1);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

PivotTable'ı veri kaynağı olarak kullanarak yeni bir Timeline ekle.

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| destCellName | String | Timeline aralığının sol üst köşesindeki hücre adı. |
| baseFieldIndex | Int32 | PivotTable.BaseFields içindeki PivotField'ın dizini |

### Dönüş Değeri

Yeni eklenen Timeline dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Date");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue(new DateTime(2023, 1, 1));
            cells["B2"].PutValue("A");
            cells["C2"].PutValue(100);
            
            cells["A3"].PutValue(new DateTime(2023, 1, 2));
            cells["B3"].PutValue("B");
            cells["C3"].PutValue(200);
            
            cells["A4"].PutValue(new DateTime(2023, 1, 3));
            cells["B4"].PutValue("A");
            cells["C4"].PutValue(150);

            // Özet tablo oluştur
            int pivotIndex = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Pivot tabloya alan ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Özet tablo verilerini yenile
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // \"Date\" alanı için temel alan dizinini bul
            int dateFieldIndex = -1;
            for (int i = 0; i < pivotTable.BaseFields.Count; i++)
            {
                if (pivotTable.BaseFields[i].Name == "Date")
                {
                    dateFieldIndex = i;
                    break;
                }
            }

            // Bulunan dizini kullanarak timeline ekle
            if (dateFieldIndex >= 0)
            {
                sheet.Timelines.Add(pivotTable, "H2", dateFieldIndex);
            }

            // Sonucu kaydet
            workbook.Save("TimelineCollectionMethodAddWithPivotTableStringInt32Demo_output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

PivotTable'ı veri kaynağı olarak kullanarak yeni bir Timeline ekle.

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| satır | Int32 | Timeline aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | Int32 | Timeline aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| baseField | PivotField | PivotTable.BaseFields içindeki PivotField |

### Dönüş Değeri

Yeni eklenen Timeline dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri oluştur
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 2, 1);
            cells["C4"].Value = 200;

            // Özet tablo oluştur
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            
            // pivot alanları ekle
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);
            pivot.AddFieldToArea(PivotFieldType.Column, pivot.BaseFields[1]);
            pivot.AddFieldToArea(PivotFieldType.Data, pivot.BaseFields[2]);

            // Pivot tabloyu kullanarak timeline ekle
            sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
            
            // Çalışma kitabını kaydedin
            workbook.Save("TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

PivotTable'ı veri kaynağı olarak kullanarak yeni bir Timeline ekle.

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| destCellName | String | Timeline aralığının sol üst köşesindeki hücre adı. |
| baseField | PivotField | PivotTable.BaseFields içindeki PivotField |

### Dönüş Değeri

Yeni eklenen Timeline dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri oluştur
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;

            // Özet tablo oluştur
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivot.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Pivot tabloyu veri kaynağı olarak kullanarak timeline ekle
            sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[0]);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


