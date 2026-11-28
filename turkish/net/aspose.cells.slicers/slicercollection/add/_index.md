---
title: "SlicerCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SlicerCollection yöntemi. PivotTable'ı veri kaynağı olarak kullanarak yeni bir Slicer ekle"
type: docs
url: /tr/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

PivotTable'ı veri kaynağı olarak kullanarak yeni bir Slicer ekle

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| destCellName | String | Slicer aralığının sol üst köşesindeki hücre. |
| baseFieldName | String | PivotTable.BaseFields içindeki PivotField'ın adı |

### Dönüş Değeri

Yeni eklenen Slicer dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri oluştur
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Özet tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];

            // Slicer ekle
            int slicerIndex = worksheet.Slicers.Add(pivot, "E3", "fruit");
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

PivotTable'ı veri kaynağı olarak kullanarak yeni bir Slicer ekle

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| satır | Int32 | Slicer aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | Int32 | Slicer aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| baseFieldName | String | PivotTable.BaseFields içindeki PivotField'ın adı |

### Dönüş Değeri

Yeni eklenen Slicer dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri oluştur
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Fruit");
            cells["B1"].PutValue("Quantity");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(50);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(30);

            // Özet tablo oluştur
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Slicer ekle
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivotTable, 20, 12, "fruit");

            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

PivotTable'ı veri kaynağı olarak kullanarak yeni bir Slicer ekle

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| satır | Int32 | Slicer aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | Int32 | Slicer aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| baseFieldIndex | Int32 | PivotTable.BaseFields içindeki PivotField'ın dizini |

### Dönüş Değeri

Yeni eklenen Slicer dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri oluştur
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Pivot tablo ekle
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Pivot tablo için slicer ekle
            int slicerIndex = worksheet.Slicers.Add(pivot, 20, 8, 0);
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

PivotTable'ı veri kaynağı olarak kullanarak yeni bir Slicer ekle

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| destCellName | String | Slicer aralığının sol üst köşesindeki hücre. |
| baseFieldIndex | Int32 | PivotTable.BaseFields içindeki PivotField'ın dizini |

### Dönüş Değeri

Yeni eklenen Slicer dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri oluştur
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // Özet tablo oluştur
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Slicer ekle
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "A1", 0);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

PivotTable'ı veri kaynağı olarak kullanarak yeni bir Slicer ekle

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| satır | Int32 | Slicer aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | Int32 | Slicer aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| baseField | PivotField | PivotTable.BaseFields içindeki PivotField |

### Dönüş Değeri

Yeni eklenen Slicer dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri oluştur
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 7;

            // Özet tablo oluştur
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // pivot alanları ekle
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Slicer ekle
            int slicerIndex = sheet.Slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Çalışma kitabını kaydedin
            workbook.Save("SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

PivotTable'ı veri kaynağı olarak kullanarak yeni bir Slicer ekle

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | PivotTable | PivotTable nesnesi |
| destCellName | String | Slicer aralığının sol üst köşesindeki hücre. |
| baseField | PivotField | PivotTable.BaseFields içindeki PivotField |

### Dönüş Değeri

Yeni eklenen Slicer dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 20;
            cells["B4"].Value = 30;

            // Özet tablo oluştur
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);

            // Slicer ekle
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "I3", pivot.BaseFields[0]);

            // Çalışma kitabını kaydedin
            workbook.Save("SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Veri kaynağı olarak ListObjet kullanan yeni bir Slicer ekle

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tablo | ListObject | ListObject nesnesi |
| indeks | Int32 | ListObject.ListColumns içinde ListColumn'un indeksi |
| destCellName | String | Slicer aralığının sol üst köşesindeki hücre. |

### Dönüş Değeri

Yeni eklenen Slicer dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ve liste nesnesi oluştur
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue("E38");
            worksheet.Cells["A3"].PutValue("E39");
            worksheet.Cells["A4"].PutValue("E40");
            
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // Liste nesnesi için slicer ekle - not: Slicers.Add bir int indeks döndürür
            int slicerIndex = worksheet.Slicers.Add(listObject, 0, "E38");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Çalışma kitabını kaydedin
            workbook.Save("SlicerCollectionMethodAddWithListObjectInt32StringDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Veri kaynağı olarak ListObjet kullanan yeni bir Slicer ekle

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tablo | ListObject | ListObject nesnesi |
| listColumn | ListColumn | ListObject.ListColumns içindeki ListColumn |
| destCellName | String | Slicer aralığının sol üst köşesindeki hücre. |

### Dönüş Değeri

Yeni eklenen Slicer dizini

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");

            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];

            SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(table, table.ListColumns[1], "I38");

            worksheet.Cells.SetColumnWidth(0, 20);
            worksheet.Cells.SetColumnWidth(1, 20);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Veri kaynağı olarak ListObjet kullanan yeni bir Slicer ekle

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tablo | ListObject | ListObject nesnesi |
| listColumn | ListColumn | ListObject.ListColumns içindeki ListColumn |
| satır | Int32 | Slicer aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | Int32 | Slicer aralığının sol üst köşesindeki hücrenin sütun indeksi. |

### Dönüş Değeri

Yeni eklenen Slicer dizini

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnInt32Int32Demo
    {
        public static void Run()
        {
            // Çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Tablo için örnek veri ekle
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue("CatA");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue("CatB");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue("CatA");
            
            // Tablo aralığını oluştur
            int endRow = 4;
            string startCell = "A1";
            string endCell = $"B{endRow}";
            
            // Doğru aşırı yüklemeyi kullanarak tabloyu çalışma sayfasına ekle
            int tableIndex = sheet.ListObjects.Add(startCell, endCell, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium2;
            
            // Kategori sütunu için slicer ekle, konum (satır 6, sütun 1)
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(table, table.ListColumns[1], 6, 1);
            
            // Sonucu kaydedin
            workbook.Save("SlicerOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


