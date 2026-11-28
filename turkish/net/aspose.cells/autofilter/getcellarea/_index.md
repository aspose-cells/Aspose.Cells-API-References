---
title: "AutoFilter.GetCellArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "AutoFilter yöntemi. Bu AutoFilter'in uygulandığı CellArea'yı alır"
type: docs
url: /tr/net/aspose.cells/autofilter/getcellarea/
---
## GetCellArea() {#getcellarea}

Bu AutoFilter'ın uygulandığı [`CellArea`](../../cellarea/) alır.

```csharp
public CellArea GetCellArea()
```

### Dönüş Değeri

bu filtrenin uygulandığı alan

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // AutoFilter gösterimi için örnek veri doldur
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Category");
            cells["C1"].PutValue("Price");

            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue("Fruit");
            cells["C2"].PutValue(2.5);

            cells["A3"].PutValue("Carrot");
            cells["B3"].PutValue("Vegetable");
            cells["C3"].PutValue(1.2);

            cells["A4"].PutValue("Banana");
            cells["B4"].PutValue("Fruit");
            cells["C4"].PutValue(3.1);

            // Başlıklara (satır indeksi 0) AutoFilter uygula, A-C (0-2) sütunlarını kapsar
            AutoFilter autoFilter = worksheet.AutoFilter;
            autoFilter.SetRange(0, 0, 2);

            try
            {
                // AutoFilter'ın uygulandığı CellArea'yi al
                CellArea result = autoFilter.GetCellArea();

                // AutoFilter aralığının koordinatlarını çıktı olarak ver
                Console.WriteLine("AutoFilter applied to cell area:");
                Console.WriteLine($"Start Row: {result.StartRow}");
                Console.WriteLine($"Start Column: {result.StartColumn}");
                Console.WriteLine($"End Row: {result.EndRow}");
                Console.WriteLine($"End Column: {result.EndColumn}");

                // İşlevselliği göstermek için basit bir filtre uygula (isteğe bağlı)
                autoFilter.Filter(1, "Fruit"); // Filter "Category" column (index 1) for "Fruit"
                autoFilter.Refresh();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea method: {ex.Message}");
            }

            // Uygulanan AutoFilter ile çalışma kitabını kaydet
            workbook.Save("AutoFilterMethodGetCellAreaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellArea(bool) {#getcellarea_1}

Belirtilen AutoFilter'ın uygulandığı [`CellArea`](../../cellarea/) alır.

```csharp
public CellArea GetCellArea(bool refreshAppliedRange)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| refreshAppliedRange | Boolean | Uygulanan aralığın yenilenip yenilenmeyeceği. Auto filter'ın uygulanan aralığında, hücre verileri değiştiğinde son satır değişebilir. Bu bayrak doğru ise, aralığın son satırı mevcut hücre verilerine göre yeniden hesaplanacaktır. |

### Dönüş Değeri

bu filtrenin uygulandığı alan

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodGetCellAreaWithBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // AutoFilter için örnek veri hazırla
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            worksheet.Cells["A4"].PutValue("Data3");

            // AutoFilter aralığını ayarla (satır 0'dan 3'e, sütun 0)
            worksheet.AutoFilter.SetRange(0, 0, 0);

            try
            {
                // refreshAppliedRange=true ile GetCellArea'yi çağır
                CellArea result = worksheet.AutoFilter.GetCellArea(true);

                // AutoFilter'ın uygulanan aralığını göster
                Console.WriteLine($"AutoFilter Range: StartRow={result.StartRow}, " +
                    $"StartColumn={result.StartColumn}, EndRow={result.EndRow}, " +
                    $"EndColumn={result.EndColumn}");

                Console.WriteLine("GetCellArea method executed successfully with boolean parameter");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellArea: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("AutoFilterMethodGetCellAreaWithBooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


