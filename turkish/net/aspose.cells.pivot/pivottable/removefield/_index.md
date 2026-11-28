---
title: "PivotTable.RemoveField"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. Belirli alan bölgesinden bir alanı kaldırır"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/removefield/
---
## RemoveField(PivotFieldType, string) {#removefield_2}

Belirli alan bölgesinden bir alanı kaldırır

```csharp
public void RemoveField(PivotFieldType fieldType, string fieldName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | PivotFieldType | Alan bölgesi tipi. |
| fieldName | String | Temel alanlardaki ad. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk pivot tabloya eriş
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // "c" alanını Veri bölgesinden kaldır
            pivotTable.RemoveField(PivotFieldType.Data, "c");
            
            // Pivot tablo verilerini hesapla
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, int) {#removefield_1}

Belirli pivot bölgeden bir alanı kaldırır.

```csharp
public void RemoveField(PivotFieldType fieldType, int baseFieldIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | PivotFieldType | Alan bölgesi tipi. |
| baseFieldIndex | Int32 | Temel alanlardaki alan indeksi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodRemoveFieldWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Satır alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Satır alanını (indeks 0) pivot tablodan kaldır
                pivotTable.RemoveField(PivotFieldType.Row, 0);
                
                Console.WriteLine("Row field removed successfully from the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveField method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("PivotTableRemoveFieldDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, PivotField) {#removefield}

Belirli alan bölgesinden alanı kaldır

```csharp
public void RemoveField(PivotFieldType fieldType, PivotField pivotField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | PivotFieldType | alan bölgesi türü. |
| pivotField | PivotField | temel alanlardaki alan. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Kaynak Excel dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("TestFile.xlsx");
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk pivot tabloya eriş
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Pivot tablodan bir sütun alanını kaldır
            if (pivotTable.ColumnFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Column, pivotTable.ColumnFields[0]);
            }
            
            // Pivot tablodan bir veri alanını kaldır
            if (pivotTable.DataFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Data, pivotTable.DataFields[0]);
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("ModifiedPivotTable.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


