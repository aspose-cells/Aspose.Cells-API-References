---
title: "PivotTable.DataField"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable özelliği. Bir PivotTable'daki tüm veri alanlarını temsil eden bir PivotField nesnesi alır. Salt okunurdur. Yalnızca Veri bölgesinde iki veya daha fazla veri alanı olduğunda oluşturulur. Varsayılan olarak satır bölgesindedir. PivotTable.AddFieldToArea yöntemiyle satır/sütun bölgesine sürükleyebilirsiniz."
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/datafield/
---
## PivotTable.DataField property

Bir [`PivotField`](../../pivotfield/) nesnesi alır; bu nesne bir PivotTable'daki tüm veri alanlarını temsil eder. Salt okunurdur. Yalnızca Veri bölgesinde iki veya daha fazla veri alanı olduğunda oluşturulur. Varsayılan olarak satır bölgesindedir. PivotTable.AddFieldToArea() yöntemiyle satır/sütun bölgesine sürükleyebilirsiniz.

```csharp
[Obsolete("Use PivotTable.ValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotField DataField { get; }
```

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırıldı. Bunun yerine lütfen PivotTable.ValuesField özelliğini kullanın. Bu yöntem Ekim 2025'ten itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Özet tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Satır alanı ve veri alanı ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // DataField özelliklerine eriş ve değiştir
            // Konum salt okunurdur, bu yüzden diğer özellikleri göstereceğiz
            pivotTable.DataField.DisplayName = "Total Sales";
            pivotTable.DataField.NumberFormat = "#,##0";
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableDataFieldDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


