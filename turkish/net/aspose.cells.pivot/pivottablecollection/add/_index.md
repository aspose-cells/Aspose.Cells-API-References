---
title: "PivotTableCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTableCollection yöntemi. Belirtilen çalışma sayfası satır ve sütun konumunda, varsayılan seçeneklerle Excel 2007'den beri yeni modern bir PivotTable ekler"
type: docs
url: /tr/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string) {#add_2}

Belirtilen çalışma sayfası satır ve sütun konumunda, varsayılan seçeneklerle yeni modern bir PivotTable ekler (Excel 2007'den beri).

```csharp
public PivotTable Add(string sourceData, string cellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| cellName | String | PivotTable hedefi için sol üst köşe hücresinin adı. |

### Dönüş Değeri

Yeni oluşturulan PivotTable örneği.

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, PivotTableCreateOptions) {#add_3}

Belirtilen çalışma sayfası satır ve sütun konumunda, varsayılan seçeneklerle yeni modern bir PivotTable ekler (Excel 2007'den beri).

```csharp
public PivotTable Add(string sourceData, string cellName, PivotTableCreateOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| cellName | String | PivotTable hedefi için sol üst köşe hücresinin adı. |
| seçenekler | PivotTableCreateOptions | Pivot tablo oluşturma seçenekleri. |

### Dönüş Değeri

Yeni oluşturulan PivotTable örneği.

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int) {#add}

Belirtilen çalışma sayfası satır ve sütun konumunda, varsayılan seçeneklerle yeni modern bir PivotTable ekler (Excel 2007'den beri).

```csharp
public PivotTable Add(string sourceData, int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| satır | Int32 | PivotTable hedefi için sol üst köşe hücresinin sıfır tabanlı satır indeksi. |
| sütun | Int32 | PivotTable hedefi için sol üst köşe hücresinin sıfır tabanlı sütun indeksi. |

### Dönüş Değeri

Yeni oluşturulan PivotTable örneği.

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, PivotTableCreateOptions) {#add_1}

Belirtilen çalışma sayfası satır ve sütun konumunda yeni bir PivotTable ekler.

```csharp
public PivotTable Add(string sourceData, int row, int column, PivotTableCreateOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| satır | Int32 | PivotTable hedefi için sol üst köşe hücresinin sıfır tabanlı satır indeksi. |
| sütun | Int32 | PivotTable hedefi için sol üst köşe hücresinin sıfır tabanlı sütun indeksi. |
| seçenekler | PivotTableCreateOptions | PivotTable oluşturma seçenekleri. |

### Dönüş Değeri

Yeni oluşturulan PivotTable örneği.

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [PivotTableCreateOptions](../../pivottablecreateoptions/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string) {#add_9}

Miras Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String | Yeni PivotTable önbelleği için veri. |
| destCellName | String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | String | Yeni PivotTable raporunun adı. |

### Dönüş Değeri

Bu pivot tablo listesindeki dizin.

### Açıklamalar

NOT: Bu yöntem artık kullanılmamaktadır. `NewPivotTableOptions.IsXlsClassic = true` ile PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) çağrısına eşdeğerdir. Lütfen bunun yerine PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) aşırı yüklemesini kullanın. Bu yöntem, Eylül 2026'dan 12 ay sonra kaldırılacaktır. Oluşabilecek rahatsızlık için özür dileriz.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // Kaynak CSV'den bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            sourceSheet.Name = "SourceData";
            
            // Örnek veri ekleyin.
            sourceSheet.Cells["A1"].PutValue("Category");
            sourceSheet.Cells["B1"].PutValue("Value");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(10);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(20);
            sourceSheet.Cells["A4"].PutValue("A");
            sourceSheet.Cells["B4"].PutValue(30);

            // Pivot tablo çalışma sayfası oluştur
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Kaynak veri aralığını al
            Aspose.Cells.Range sourceRange = sourceSheet.Cells.MaxDisplayRange;
            string sourceData = String.Format("=SourceData!{0}", sourceRange.Address);
            
            // String, String, String parametreleriyle pivot tablo ekle
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int pivotIndex = pivotTables.Add(sourceData, "A1", "MyPivotTable");
            
            // Pivot tabloyu yapılandır
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_10}

Miras Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, string, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String | Yeni PivotTable önbelleği için veri. |
| destCellName | String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | String | Yeni PivotTable raporunun adı. |
| useSameSource | Boolean | Başka bir mevcut pivot tablo bu veri kaynağını kullandığında aynı veri kaynağının kullanılıp kullanılmayacağını gösterir. Özellik true ise, bellek tasarrufu sağlar. |

### Dönüş Değeri

Yeni eklenen önbellek indeksi.

### Açıklamalar

NOT: Bu yöntem artık kullanılmamaktadır. `NewPivotTableOptions.IsXlsClassic = true` ile PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) çağrısına eşdeğerdir. Lütfen bunun yerine PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) aşırı yüklemesini kullanın. Bu yöntem, Eylül 2026'dan 12 ay sonra kaldırılacaktır. Oluşabilecek rahatsızlık için özür dileriz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringStringStringBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Add yöntemi için parametreleri tanımla
            string sourceData = "A1:B4";
            string destCellName = "E5";
            string tableName = "FruitPivotTable";
            bool useSameSource = true;

            try
            {
                // Parametreler (String, String, String, Boolean) ile Add yöntemini çağır
                int index = worksheet.PivotTables.Add(sourceData, destCellName, tableName, useSameSource);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                Console.WriteLine($"Pivot table name: {worksheet.PivotTables[index].Name}");
                Console.WriteLine($"Pivot table location: {worksheet.PivotTables[index].TableRange1}");

                // Pivot tabloyu yapılandır
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_6}

Miras Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String | Yeni PivotTable için veri hücre aralığı. Örnek : Sheet1!A1:C8 |
| satır | Int32 | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | Int32 | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| tableName | String | Yeni PivotTable raporunun adı. |

### Dönüş Değeri

Bu pivot tablo listesindeki dizin.

### Açıklamalar

NOT: Bu yöntem artık kullanılmamaktadır. `NewPivotTableOptions.IsXlsClassic = true` ile PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) çağrısına eşdeğerdir. Lütfen bunun yerine PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) aşırı yüklemesini kullanın. Bu yöntem, Eylül 2026'dan 12 ay sonra kaldırılacaktır. Oluşabilecek rahatsızlık için özür dileriz.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Veri için bir çalışma sayfası ekle
            Worksheet dataWorksheet = workbook.Worksheets[0];
            dataWorksheet.Name = "Data";
            
            // Örnek veri ekleyin.
            dataWorksheet.Cells["A1"].PutValue("Category");
            dataWorksheet.Cells["B1"].PutValue("Product");
            dataWorksheet.Cells["C1"].PutValue("Sales");
            
            dataWorksheet.Cells["A2"].PutValue("Electronics");
            dataWorksheet.Cells["B2"].PutValue("Laptop");
            dataWorksheet.Cells["C2"].PutValue(1000);
            
            dataWorksheet.Cells["A3"].PutValue("Electronics");
            dataWorksheet.Cells["B3"].PutValue("Phone");
            dataWorksheet.Cells["C3"].PutValue(800);
            
            dataWorksheet.Cells["A4"].PutValue("Furniture");
            dataWorksheet.Cells["B4"].PutValue("Chair");
            dataWorksheet.Cells["C4"].PutValue(200);
            
            // Pivot tablo için bir çalışma sayfası ekle
            Worksheet pivotWorksheet = workbook.Worksheets.Add("PivotTable");
            
            // (String, Int32, Int32, String) parametreleriyle Add yöntemi kullanarak pivot tablo ekle
            string pivotDataRange = "Data!A1:C4";
            int row = 0;
            int column = 0;
            string tableName = "SalesPivotTable";
            
            int pivotIndex = pivotWorksheet.PivotTables.Add(pivotDataRange, row, column, tableName);
            
            // Pivot tabloya eriş
            PivotTable pivotTable = pivotWorksheet.PivotTables[pivotIndex];
            
            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Konsolidasyon işlevini ayarla
            pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
            
            // Pivot tablo verilerini yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_7}

Miras Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String | Yeni PivotTable için veri hücre aralığı. Örnek : Sheet1!A1:C8 |
| satır | Int32 | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | Int32 | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| tableName | String | Yeni PivotTable raporunun adı. |
| useSameSource | Boolean | Başka bir mevcut pivot tablo bu veri kaynağını kullandığında aynı veri kaynağının kullanılıp kullanılmayacağını gösterir. Özellik true ise, bellek tasarrufu sağlar. |

### Dönüş Değeri

Yeni eklenen önbellek indeksi.

### Açıklamalar

NOT: Bu yöntem artık kullanılmamaktadır. `NewPivotTableOptions.IsXlsClassic = true` ile PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) çağrısına eşdeğerdir. Lütfen bunun yerine PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) aşırı yüklemesini kullanın. Bu yöntem, Eylül 2026'dan 12 ay sonra kaldırılacaktır. Oluşabilecek rahatsızlık için özür dileriz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            
            // Veri aralığını tanımla
            string sourceData = "A1:C4";
            
            try
            {
                // Parametreler: (String sourceData, Int32 row, Int32 column, String tableName, Boolean useSameSource) ile Add yöntemini çağır
                int index = worksheet.PivotTables.Add(sourceData, 6, 0, "PivotTable1", false);
                
                Console.WriteLine("Pivot table added successfully at index: " + index);
                
                // Yeni oluşturulan pivot tabloya eriş
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Pivot tabloyu yapılandır
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
                pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
                pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool, bool) {#add_8}

Miras Excel 97-2003 düzeni ve stiliyle yeni bir PivotTable ekler.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String | Yeni PivotTable için veri hücre aralığı. Örnek : Sheet1!A1:C8 |
| satır | Int32 | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | Int32 | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| tableName | String | Yeni PivotTable raporunun adı. |
| useSameSource | Boolean | Başka bir mevcut pivot tablo bu veri kaynağını kullandığında aynı veri kaynağının kullanılıp kullanılmayacağını gösterir. Özellik true ise, bellek tasarrufu sağlar. |
| isXlsClassic | Boolean | Excel 97-2003 klasik pivot tablosu eklenip eklenmeyeceğini gösterir. |

### Dönüş Değeri

Yeni eklenen önbellek indeksi.

### Açıklamalar

NOT: Bu yöntem artık kullanılmamaktadır. `NewPivotTableOptions.IsXlsClassic = true` ile PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) çağrısına eşdeğerdir. Lütfen bunun yerine PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) aşırı yüklemesini kullanın. Bu yöntem, Ekim 2026'dan 12 ay sonra kaldırılacaktır. Oluşabilecek rahatsızlık için özür dileriz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringInt32Int32StringBooleanBDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Sales");
            cells["A2"].PutValue("Product1");
            cells["B2"].PutValue("North");
            cells["C2"].PutValue(1000);
            cells["A3"].PutValue("Product2");
            cells["B3"].PutValue("South");
            cells["C3"].PutValue(2000);
            cells["A4"].PutValue("Product3");
            cells["B4"].PutValue("East");
            cells["C4"].PutValue(3000);
            cells["A5"].PutValue("Product4");
            cells["B5"].PutValue("West");
            cells["C5"].PutValue(4000);

            // Kaynak veri aralığını tanımla
            string sourceData = "A1:C5";

            try
            {
                // Add yöntemini (String, Int32, Int32, String, Boolean, Boolean) parametreleriyle çağırın
                int index = worksheet.PivotTables.Add(
                    sourceData,    // String sourceData
                    3,            // Int32 row - pivot table will start at row 3
                    0,            // Int32 column - pivot table will start at column 0
                    "PivotTable1", // String tableName
                    false,        // Boolean useSameSource
                    false         // Boolean isXlsClassic
                );

                Console.WriteLine("Pivot table added successfully at index: " + index);

                // Pivot tabloyu yapılandır
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, bool, bool) {#add_11}

Yeni bir PivotTable ekler.

```csharp
[Obsolete("Use PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) overload instead. This method is equivalent to setting NewPivotTableOptions.IsXlsClassic = true.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(string sourceData, string cell, string tableName, bool useSameSource, 
    bool isXlsClassic)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String | Yeni PivotTable için veri hücre aralığı. Örnek : Sheet1!A1:C8 |
| hücre | String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | String | Yeni PivotTable raporunun adı. |
| useSameSource | Boolean | Başka bir mevcut pivot tablosu bu veri kaynağını kullandığında aynı veri kaynağının kullanılıp kullanılmadığını gösterir. Özellik true ise, aynı veri kaynağı bir pivot önbelleğinde toplandığında bellek tasarrufu sağlar. |
| isXlsClassic | Boolean | Excel 97-2003 klasik pivot tablosu eklenip eklenmeyeceğini gösterir. |

### Dönüş Değeri

Yeni eklenen önbellek indeksi.

### Açıklamalar

NOT: Bu yöntem artık kullanılmamaktadır. `NewPivotTableOptions.IsXlsClassic = true` ile PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) çağrısına eşdeğerdir. Lütfen bunun yerine PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) aşırı yüklemesini kullanın. Bu yöntem, Ekim 2026'dan 12 ay sonra kaldırılacaktır. Oluşabilecek rahatsızlık için özür dileriz.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodAddWithStringStringStringBooleanBooleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek verileri doldur
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            for (int i = 2; i <= 10; i++)
            {
                cells["A" + i].PutValue("Cat" + (i % 3 + 1));
                cells["B" + i].PutValue("Prod" + i);
                cells["C" + i].PutValue(i * 100);
            }

            // Belirtilen parametrelerle pivot tablo ekle
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E1", "SalesPivot", false, false);
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Pivot tabloyu yapılandır
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0); // Category as row
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2); // Sum of Sales
            
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Başka bir PivotTable üzerine yeni bir PivotTable ekler.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotTable | PivotTable | Kaynak pivotTable. |
| destCellName | String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | String | Yeni PivotTable raporunun adı. |

### Dönüş Değeri

Yeni eklenen PivotTable dizini.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Veri aralığından bir pivot tablo oluştur
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];

            try
            {
                // Add yöntemini (PivotTable, String, String) parametreleriyle çağırın
                int newPivotIndex = pivotTables.Add(sourcePivotTable, "E10", "PivotTable2");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Etkisini göstermek için çalışma kitabını kaydedin
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableStringStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_4}

Başka bir PivotTable üzerine yeni bir PivotTable ekler.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotTable | PivotTable | Kaynak pivotTable. |
| satır | Int32 | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | Int32 | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| tableName | String | Yeni PivotTable raporunun adı. |

### Dönüş Değeri

Yeni eklenen PivotTable dizini.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Kaynak bir pivot tablo oluştur
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "C3", "SourcePivotTable");
            PivotTable sourcePivotTable = pivotTables[pivotIndex];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // Add yöntemini (PivotTable, Int32, Int32, String) parametreleriyle çağırın
                int newPivotIndex = pivotTables.Add(sourcePivotTable, 10, 5, "NewPivotTable");
                Console.WriteLine($"New pivot table added at index: {newPivotIndex}");

                // Etkisini göstermek için çalışma kitabını kaydedin
                workbook.Save("PivotTableCollectionMethodAddWithPivotTableInt32Int32StringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_13}

Birden fazla konsolidasyon aralığını veri kaynağı olarak kullanarak koleksiyona yeni bir PivotTable Nesnesi ekler.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String[] | Birden fazla konsolidasyon aralığı, örneğin {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Tek bir sayfa alanının otomatik oluşturulup oluşturulmayacağını belirler. True ise, aşağıdaki pageFields parametresi yok sayılacaktır. |
| pageFields | PivotPageFields | Pivot sayfa alanı öğeleri. |
| destCellName | String | destCellName Yeni PivotTable raporunun adı. |
| tableName | String | yeni PivotTable raporunun adı. |

### Dönüş Değeri

Yeni eklenen PivotTable dizini.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;

            // Veri aralığını tanımla
            string[] sourceData = { "A1:C4" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            string destCellName = "E5";
            string tableName = "PivotTable1";

            try
            {
                // Belirtilen parametrelerle Add yöntemini çağır
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, destCellName, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Yeni oluşturulan pivot tabloya eriş
                PivotTable pivotTable = worksheet.PivotTables[index];
                
                // Pivot tablo alanlarını yapılandırın
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_12}

Birden fazla konsolidasyon aralığını veri kaynağı olarak kullanarak koleksiyona yeni bir PivotTable Nesnesi ekler.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | String[] | Birden fazla konsolidasyon aralığı, örneğin {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Tek bir sayfa alanının otomatik oluşturulup oluşturulmayacağını belirler. True ise, aşağıdaki pageFields parametresi yok sayılacaktır. |
| pageFields | PivotPageFields | Pivot sayfa alanı öğeleri. |
| satır | Int32 | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | Int32 | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| tableName | String | Yeni PivotTable raporunun adı. |

### Dönüş Değeri

Yeni eklenen PivotTable dizini.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionMethodAddWithStringBooleanPivotPageFieldsDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 2000;
            
            cells["A4"].Value = "Product3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 3000;
            
            cells["A5"].Value = "Product1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 4000;
            
            cells["A6"].Value = "Product2";
            cells["B6"].Value = "North";
            cells["C6"].Value = 5000;

            // Add yöntemi için parametreleri tanımla
            string[] sourceData = { "A1:C6" };
            bool isAutoPage = true;
            PivotPageFields pageFields = new PivotPageFields();
            int row = 8;
            int column = 1;
            string tableName = "PivotTable1";

            try
            {
                // Belirtilen parametrelerle Add yöntemini çağır
                int index = worksheet.PivotTables.Add(sourceData, isAutoPage, pageFields, row, column, tableName);
                
                Console.WriteLine($"Pivot table added successfully at index: {index}");
                
                // Pivot tabloyu yapılandır
                PivotTable pivotTable = worksheet.PivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
                
                // Verileri yenileyin
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("PivotTableAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotPageFields](../../pivotpagefields/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


