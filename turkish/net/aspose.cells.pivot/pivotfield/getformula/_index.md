---
title: "PivotField.GetFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotField yöntemi. Hesaplanmış alanın formülünü alır. Yalnızca hesaplanmış alan için çalışır"
type: docs
url: /tr/net/aspose.cells.pivot/pivotfield/getformula/
---
## PivotField.GetFormula method

Hesaplanmış alanın formülünü alır. Yalnızca hesaplanmış alan için çalışır.

```csharp
public string GetFormula()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetFormulaDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;
            
            // Özet tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Formülle hesaplanmış alan ekle
            pivotTable.AddCalculatedField("=ABS('Sales')", "Absolute Sales");
            
            // Hesaplanmış alandan formülü al
            PivotFieldCollection fields = pivotTable.DataFields;
            string formula = fields[fields.Count - 1].GetFormula();
            
            // Formülü çıktı olarak ver
            Console.WriteLine("Calculated field formula: " + formula);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


