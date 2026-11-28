---
title: "PivotAreaCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotAreaCollection yöntemi. Pivot alanı ekler"
type: docs
url: /tr/net/aspose.cells.pivot/pivotareacollection/add/
---
## Add(PivotArea) {#add}

Pivot alanı ekler.

```csharp
[Obsolete("Use PivotAreaCollection.AddPivotArea(PivotArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(PivotArea pivotArea)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivotArea | PivotArea | Pivot alanı. |

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen AddPivotArea() yöntemini kullanın. Bu yöntem, Aralık 2025'ten itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotAreaCollectionMethodAddWithPivotAreaDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("PivotTable");
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);

            // Pivot tablo ekle
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
            
            // Pivot alanlarına alanlar ekleyin
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Koşullu biçim oluşturun
            PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;

            // Pivot alanı oluşturun ve koleksiyona ekleyin
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Value");
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            pcf.PivotAreas.Add(pivotArea);

            // Biçim koşulu ekleyin
            FormatCondition fc = pcf.FormatConditions[pcf.FormatConditions.AddCondition(FormatConditionType.CellValue)];
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Formula1 = "15";
            fc.Style.BackgroundColor = Color.Yellow;

            // Verileri hesaplayın ve kaydedin
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            workbook.Save("PivotAreaCollectionMethodAddWithPivotAreaDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotArea](../../pivotarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

Pivot tablo görünümüne dayalı bir alan ekler.

```csharp
public void Add(CellArea cellArea)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | CellArea | Pivot tablo görünümüne dayalı alan. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaCollectionMethodAddWithCellAreaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri oluştur
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Bir pivot tablo ekle
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Pivot alanlarına eklemek için bir hücre alanı tanımlayın
            CellArea cellArea = new CellArea();
            cellArea.StartRow = 0;
            cellArea.StartColumn = 0;
            cellArea.EndRow = 2;
            cellArea.EndColumn = 1;

            // Alanı seçerek pivot alanı koleksiyonunu alın
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(cellArea);

            try
            {
                // Add yöntemini CellArea parametresiyle çağırın
                pivotAreas.Add(cellArea);

                Console.WriteLine("Pivot area added successfully for cell area: " +
                    $"({cellArea.StartRow},{cellArea.StartColumn}) to ({cellArea.EndRow},{cellArea.EndColumn})");

                // Eklenen pivot alanlarını gösterin
                foreach (PivotArea area in pivotAreas)
                {
                    CellArea[] areas = area.GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Pivot area covers: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("PivotAreaCollectionMethodAddWithCellAreaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


