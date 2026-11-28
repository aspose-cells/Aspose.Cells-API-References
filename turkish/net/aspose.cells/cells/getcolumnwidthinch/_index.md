---
title: "Cells.GetColumnWidthInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen sütunun normal görünümde inç cinsinden genişliğini alır"
type: docs
url: /tr/net/aspose.cells/cells/getcolumnwidthinch/
---
## Cells.GetColumnWidthInch method

Belirtilen sütunun normal görünümde, inç biriminde genişliğini alır.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double GetColumnWidthInch(int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi |

### Dönüş Değeri

Sütun genişliği

Normal görünümde sütunun genişliği.

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Cells.GetColumnWidth(int ,bool , CellsUnitType ) yöntemini kullanın. Bu yöntem, Nisan 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthInchWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Gösterim için sütun genişliğini inç olarak ayarla
            int columnIndex = 2;
            cells.SetColumnWidthInch(columnIndex, 2.5);

            try
            {
                // Int32 parametresiyle GetColumnWidthInch'i çağır
                double columnWidth = cells.GetColumnWidthInch(columnIndex);

                // Sonucu göster
                Console.WriteLine($"Width of column {columnIndex} in inches: {columnWidth}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthInch method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CellsMethodGetColumnWidthInchDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


