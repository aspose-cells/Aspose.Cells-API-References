---
title: "PivotTable.AddFieldToArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. Alanı belirli bir alana ekler"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/addfieldtoarea/
---
## AddFieldToArea(PivotFieldType, string) {#addfieldtoarea_2}

Alanı belirli alana ekler.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, string fieldName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | PivotFieldType | Alan bölgesi tipi. |
| fieldName | String | Temel alanlardaki ad. |

### Dönüş Değeri

Belirli alanlardaki alan konumu. Eğer böyle adlandırılmış bir alan yoksa, -1 döndürülür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "P1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "P2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 1500;
            cells["A4"].Value = "P3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 2000;
            cells["A5"].Value = "P1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 1200;

            // Bir pivot tablo ekle
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[index];

            // AddFieldToArea kullanarak dize alan adlarıyla farklı alanlara alanlar ekle
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Column, "Region");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Özet tabloyu yenile ve hesapla
            pivot.RefreshData();
            pivot.CalculateData();

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableDemo_out.xlsx");
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

## AddFieldToArea(PivotFieldType, int) {#addfieldtoarea_1}

Alanı belirli alana ekler.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, int baseFieldIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | PivotFieldType | Alan bölgesi tipi. |
| baseFieldIndex | Int32 | Temel alanlardaki dizin. |

### Dönüş Değeri

Belirli alanlardaki alan konumu.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // PivotTable için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Product " + (i % 3 + 1));
                worksheet.Cells["B" + i].PutValue("Region " + (i % 2 + 1));
                worksheet.Cells["C" + i].PutValue(i * 100);
            }

            // Bir PivotTable ekle.
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // AddFieldToArea(PivotFieldType, Int32) kullanarak alanları bölgelere ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row field
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data field

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableDemo_out.xlsx");
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

## AddFieldToArea(PivotFieldType, PivotField) {#addfieldtoarea}

Alanı belirli alana ekler.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, PivotField pivotField)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | PivotFieldType | alan bölgesi türü. |
| pivotField | PivotField | temel alanlardaki alan. |

### Dönüş Değeri

Belirli alanlardaki alan konumu.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Kaynak verileri içeren bir çalışma sayfası ekle
            Worksheet sourceSheet = workbook.Worksheets[0];
            sourceSheet.Name = "Source Data";
            
            // Örnek veri ekleyin.
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Region");
            sourceSheet.Cells["C1"].PutValue("Sales");
            
            sourceSheet.Cells["A2"].PutValue("Product A");
            sourceSheet.Cells["B2"].PutValue("North");
            sourceSheet.Cells["C2"].PutValue(1000);
            
            sourceSheet.Cells["A3"].PutValue("Product B");
            sourceSheet.Cells["B3"].PutValue("South");
            sourceSheet.Cells["C3"].PutValue(2000);
            
            sourceSheet.Cells["A4"].PutValue("Product A");
            sourceSheet.Cells["B4"].PutValue("East");
            sourceSheet.Cells["C4"].PutValue(1500);
            
            sourceSheet.Cells["A5"].PutValue("Product B");
            sourceSheet.Cells["B5"].PutValue("West");
            sourceSheet.Cells["C5"].PutValue(2500);

            // Bir pivot tablo ekle
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            string source = "='Source Data'!A1:C5";
            int index = pivotTables.Add(source, "A1", "PivotTable");
            PivotTable pTable = pivotTables[index];

            // Alanları bölgelere ekle
            pTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pTable.AddFieldToArea(PivotFieldType.Row, 1); // Region
            
            // Veri alanı ekle
            pTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pTable.DataFields[0].Function = ConsolidationFunction.Sum;
            pTable.DataFields[0].NumberFormat = "$0.00";

            // PivotField parametresi kullanarak veri alanını sütun alanına ekle
            if (pTable.DataField != null)
            {
                pTable.AddFieldToArea(PivotFieldType.Column, pTable.DataField);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableDemo.xlsx");
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


