---
title: "PivotTable.AddCalculatedField"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. Pivot alana hesaplanmış bir alan ekler"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/addcalculatedfield/
---
## AddCalculatedField(string, string, bool) {#addcalculatedfield_1}

Pivot alanına hesaplanmış bir alan ekler.

```csharp
public void AddCalculatedField(string name, string formula, bool dragToDataArea)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Hesaplanmış alanın adı |
| formül | String | Hesaplanmış alanın formülü. |
| dragToDataArea | Boolean | True,bu alanı veri alanına hemen sürükle |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddCalculatedFieldWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "A";
            cells["B2"].Value = 100;
            cells["A3"].Value = "B";
            cells["B3"].Value = 150;
            cells["A4"].Value = "C";
            cells["B4"].Value = 200;

            // Özet tablo oluştur
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Hesaplanmış alan ekle
            pivotTable.AddCalculatedField("DoubleSales", "=Sales*2", true);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableWithCalculatedField.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddCalculatedField(string, string) {#addcalculatedfield}

Pivot alanına hesaplanmış bir alan ekler ve veri alanına sürükler.

```csharp
public void AddCalculatedField(string name, string formula)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Hesaplanmış alanın adı |
| formül | String | Hesaplanmış alanın formülü. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddCalculatedFieldWithStringStringDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(8);
            
            worksheet.Cells["C1"].PutValue("Quantity");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(3);
            worksheet.Cells["C4"].PutValue(10);

            // Özet tablo koleksiyonu oluştur
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Pivot tablo ekle ve indeksini al
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            
            // Pivot tablo nesnesini al
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Satır alanına alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Veri alanları ekle
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Hesaplanmış alan ekle
            pivotTable.AddCalculatedField("Total", "=Price*Quantity");
            
            // Veri alanını biçimlendir
            pivotTable.DataFields["Total"].NumberFormat = "$#,##0.00";
            
            // Özet tabloyu yenile ve hesapla
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableWithCalculatedField.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


