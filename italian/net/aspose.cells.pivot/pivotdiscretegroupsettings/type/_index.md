---
title: "PivotDiscreteGroupSettings.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotDiscreteGroupSettings. Ottiene il tipo di gruppo"
type: docs
url: /it/net/aspose.cells.pivot/pivotdiscretegroupsettings/type/
---
## PivotDiscreteGroupSettings.Type property

Ottiene il tipo di gruppo.

```csharp
public override PivotFieldGroupType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDiscreteGroupSettingsPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio
            worksheet.Cells[0, 0].PutValue("Item");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Raggruppa gli elementi
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { 
                new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }) 
            }, true);

            // Ottieni le impostazioni del gruppo e dimostra la proprietà Type
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;
            Console.WriteLine("Group Type: " + groupSettings.Type);

            workbook.Save("PivotDiscreteGroupSettingsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotDiscreteGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


