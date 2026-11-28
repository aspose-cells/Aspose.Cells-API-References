---
title: "PivotTable.Fields"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotTable yöntemi. Alan tipine göre belirli alanları alır"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/fields/
---
## PivotTable.Fields method

Alan tipine göre belirli alanları alır.

```csharp
[Obsolete("Use PivotField.GetFields(PivotFieldType) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotFieldCollection Fields(PivotFieldType fieldType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fieldType | PivotFieldType | alan tipi. |

### Dönüş Değeri

belirli alan koleksiyonu

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen PivotField.GetFields(PivotFieldType) yöntemini kullanın. Bu yöntem Mayıs 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFieldsWithPivotFieldTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = "Sheet";

            // Örnek veri
            ws.Cells[0, 0].PutValue("X");
            ws.Cells[0, 1].PutValue("Y");
            ws.Cells[0, 2].PutValue("Data");

            ws.Cells[1, 0].PutValue("A");
            ws.Cells[1, 1].PutValue("C");
            ws.Cells[1, 2].PutValue(10);

            ws.Cells[2, 0].PutValue("A");
            ws.Cells[2, 1].PutValue("D");
            ws.Cells[2, 2].PutValue(25);

            ws.Cells[3, 0].PutValue("B");
            ws.Cells[3, 1].PutValue("C");
            ws.Cells[3, 2].PutValue(30);

            ws.Cells[4, 0].PutValue("B");
            ws.Cells[4, 1].PutValue("D");
            ws.Cells[4, 2].PutValue(45);

            // Özet tablo oluştur
            PivotTableCollection ptc = ws.PivotTables;
            int index = ptc.Add("=Sheet!A1:C5", "A7", "PivotTable1");
            PivotTable pt = ptc[index];

            // Alanları ekleyin ve PivotFieldType ile Fields yöntemini gösterin
            int fp = pt.AddFieldToArea(PivotFieldType.Row, "X");
            PivotField rowField = pt.Fields(PivotFieldType.Row)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Column, "Y");
            PivotField colField = pt.Fields(PivotFieldType.Column)[fp];

            fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
            PivotField dataField = pt.Fields(PivotFieldType.Data)[fp];

            // Yüzde hesaplamalı ikinci veri alanını ekleyin
            fp = pt.AddFieldToArea(PivotFieldType.Data, "Data");
            dataField = pt.Fields(PivotFieldType.Data)[fp];
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfColumn;

            pt.AddFieldToArea(PivotFieldType.Column, pt.DataField);
            pt.RefreshData();
            pt.CalculateData();

            wb.Save("PivotTableFieldsDemo.xlsx");
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


