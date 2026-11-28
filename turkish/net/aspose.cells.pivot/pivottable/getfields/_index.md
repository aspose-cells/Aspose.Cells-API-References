---
title: "PivotTable.GetFields"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. Bölgeye göre belirli pivot alan listesini alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/getfields/
---
## PivotTable.GetFields method

Bölgeye göre belirli pivot alan listesini alır.

```csharp
public PivotFieldCollection GetFields(PivotFieldType fieldType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | PivotFieldType | bölge türü. |

### Dönüş Değeri

belirli pivot alan koleksiyonu

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodGetFieldsWithPivotFieldTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;

            // Bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            try
            {
                // GetFields yöntemini PivotFieldType.Row parametresiyle çağır
                PivotFieldCollection rowFields = pivotTable.GetFields(PivotFieldType.Row);
                
                Console.WriteLine($"Number of row fields: {rowFields.Count}");
                foreach (PivotField field in rowFields)
                {
                    Console.WriteLine($"Row field name: {field.Name}");
                }

                // GetFields yöntemini PivotFieldType.Data parametresiyle çağır
                PivotFieldCollection dataFields = pivotTable.GetFields(PivotFieldType.Data);
                
                Console.WriteLine($"Number of data fields: {dataFields.Count}");
                foreach (PivotField field in dataFields)
                {
                    Console.WriteLine($"Data field name: {field.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFields method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableGetFieldsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotFieldCollection](../../pivotfieldcollection/)
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


