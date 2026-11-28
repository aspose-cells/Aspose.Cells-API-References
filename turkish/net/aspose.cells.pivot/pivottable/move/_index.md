---
title: "PivotTable.Move"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. PivotTable'ı çalışma sayfasında farklı bir konuma taşır"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/move/
---
## Move(int, int) {#move}

PivotTable'ı çalışma sayfasında farklı bir konuma taşır.

```csharp
[Obsolete("Use PivotTable.MoveTo() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | satır indeksi. |
| sütun | Int32 | sütun indeksi. |

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine lütfen PivotTable.MoveTo() yöntemini kullanın. Bu yöntem Aralık 2024'ten itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveWithInt32Int32Demo
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
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Bir pivot tablo oluştur
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Pivot tabloya alanlar ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Pivot tabloyu doldurmak için verileri hesapla
            pivotTable.CalculateData();

            Console.WriteLine("Pivot table created at E3");

            try
            {
                // Pivot tabloyu yeni konuma taşı (satır 10, sütun 5)
                pivotTable.Move(10, 5);
                Console.WriteLine("Pivot table moved to row 10, column 5");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("PivotTableMethodMoveWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(string) {#move_1}

PivotTable'ı çalışma sayfasında farklı bir konuma taşır.

```csharp
[Obsolete("Use PivotTable.MoveTo() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(string destCellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| destCellName | String | hedef hücre adı. |

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırıldı. Bunun yerine lütfen PivotTable.MoveTo() yöntemini kullanın. Bu yöntem Aralık 2024'ten itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodMoveWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 200;

            // Özet tablo oluştur
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Pivot tabloya alan ekle
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            try
            {
                // Pivot tabloyu hücre adı kullanarak yeni bir konuma taşı
                pivotTable.Move("G10");

                Console.WriteLine("PivotTable moved successfully to G10");
                Console.WriteLine($"New location: {pivotTable.TableRange1.StartRow}, {pivotTable.TableRange1.StartColumn}");

                // Çalışma kitabını kaydedin
                workbook.Save("PivotTableMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error moving PivotTable: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


