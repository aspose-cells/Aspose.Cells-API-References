---
title: "PivotArea.SelectField"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotArea yöntemi. Bölgedeki bir alanı alan olarak seç"
type: docs
url: /tr/net/aspose.cells.pivot/pivotarea/selectfield/
---
## SelectField(PivotFieldType, string) {#selectfield_1}

Bölgede bir alanı alan olarak seç.

```csharp
public void SelectField(PivotFieldType axisType, string fieldName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| axisType | PivotFieldType | Bölge türü. |
| fieldName | String | Pivot alanının adı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodSelectFieldWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["C2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Phone");
            worksheet.Cells["C3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Clothing");
            worksheet.Cells["B4"].PutValue("Shirt");
            worksheet.Cells["C4"].PutValue(50);

            // Pivot tablo ekle
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Pivot alanlarına alanlar ekleyin
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Koşullu biçim oluşturun
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;

            // SelectField'i PivotFieldType ve string parametreleriyle göster
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Sales");
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            pcf.PivotAreas.Add(pivotArea);

            // Çalışma kitabını kaydedin
            workbook.Save("PivotAreaSelectFieldDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SelectField(PivotFieldType, PivotField) {#selectfield}

Bölgede bir alanı alan olarak seç.

```csharp
public void SelectField(PivotFieldType axisType, PivotField field)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| axisType | PivotFieldType | Bölge türü. |
| alan | PivotField | Pivot alanı. |

### Örnekler

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodSelectFieldWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            byte[] SrcDataByteArray = Encoding.ASCII.GetBytes(
@"City,Product,Sales
Paris,Cream,2300
Paris,Lotion,1600
Tunis,Cream,900
Tunis,Lotion,1400
Tunis,Cream,3090
Tunis,Lotion,6000
Paris,Cream,4320");

            using (MemoryStream dataStream = new MemoryStream(SrcDataByteArray))
            {
                Workbook wb = new Workbook(dataStream, new LoadOptions(LoadFormat.Csv));
                Worksheet sheet = wb.Worksheets[0];
                
                PivotTableCollection pivotTables = sheet.PivotTables;
                int pivotIndex = pivotTables.Add("=A1:C8", "F3", "MyPivotTable");
                PivotTable pivotTable = pivotTables[pivotIndex];

                pivotTable.AddFieldToArea(PivotFieldType.Column, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 2);

                int formatIndex = pivotTable.ConditionalFormats.Add();
                PivotConditionalFormat pivotFormat = pivotTable.ConditionalFormats[formatIndex];
                pivotFormat.ScopeType = PivotConditionFormatScopeType.Data;

                PivotArea pivotArea = new PivotArea(pivotTable);
                pivotArea.SelectField(PivotFieldType.Data, pivotTable.DataFields[0]);
                pivotFormat.PivotAreas.Add(pivotArea);

                int conditionIndex = pivotFormat.FormatConditions.AddCondition(
                    FormatConditionType.CellValue, 
                    OperatorType.GreaterThan, 
                    "1", 
                    null);
                pivotFormat.FormatConditions[conditionIndex].Style.BackgroundColor = System.Drawing.ColorTranslator.FromHtml("#e39e9e");

                wb.Save("output.xlsx");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


