---
title: "CellsHelper.GetDateTimeFromDouble"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Double değerini tarih saat değerine dönüştür."
type: docs
url: /tr/net/aspose.cells/cellshelper/getdatetimefromdouble/
---
## CellsHelper.GetDateTimeFromDouble method

Double değerini tarih saat değerine dönüştür.

```csharp
public static DateTime GetDateTimeFromDouble(double doubleValue, bool date1904)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| doubleValue | Double | Double değeri. |
| date1904 | Boolean | 1904 tarih sistemi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodGetDateTimeFromDoubleWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yöntem parametreleri için verileri hazırla (Double, Boolean)
            double doubleValue = 44197.5; // Represents 2021-01-01 12:00:00 in Excel serial date format
            bool date1904 = false; // Using 1900 date system

            try
            {
                // GetDateTimeFromDouble yöntemini belirli parametre tipleriyle çağır
                DateTime result = CellsHelper.GetDateTimeFromDouble(doubleValue, date1904);
                
                // Sonucu göster
                Console.WriteLine($"Converted DateTime: {result}");
                
                // Sonucu bir hücreye yaz
                worksheet.Cells["A1"].PutValue("Original Double Value:");
                worksheet.Cells["B1"].PutValue(doubleValue);
                worksheet.Cells["A2"].PutValue("Converted DateTime:");
                worksheet.Cells["B2"].PutValue(result.ToString());
                
                Console.WriteLine("Method executed successfully with parameters (Double, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDateTimeFromDouble method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("MethodGetDateTimeFromDoubleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


