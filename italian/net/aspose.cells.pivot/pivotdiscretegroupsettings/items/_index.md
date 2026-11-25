---
title: "PivotDiscreteGroupSettings.Items"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotDiscreteGroupSettings. Ottiene gli elementi discreti"
type: docs
url: /it/net/aspose.cells.pivot/pivotdiscretegroupsettings/items/
---
## PivotDiscreteGroupSettings.Items property

Ottiene gli elementi discreti.

```csharp
[Obsolete("Use PivotField.GroupBy(DiscreteGroupItem[], bool) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomPiovtFieldGroupItem[] Items { get; }
```

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.GroupBy(DiscreteGroupItem[], bool). Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDiscreteGroupSettingsPropertyItemsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Apple");
            worksheet.Cells["A6"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["B5"].PutValue(150);
            worksheet.Cells["B6"].PutValue(250);

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Ottieni il campo pivot e raggruppalo
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[0], false);

            // Accedi alle impostazioni del gruppo discreto
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;

            // Visualizza gli elementi correnti
            Console.WriteLine("Current Items count: " + groupSettings.Items.Length);
            foreach (CustomPiovtFieldGroupItem item in groupSettings.Items)
            {
                Console.WriteLine("Item: " + item.ToString());
            }

            // Salva la cartella di lavoro
            workbook.Save("PivotDiscreteGroupSettingsItemsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotDiscreteGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


