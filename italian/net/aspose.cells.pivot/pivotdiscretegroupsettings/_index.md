---
title: "Class PivotDiscreteGroupSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Pivot.PivotDiscreteGroupSettings class. Rappresenta il gruppo discreto del campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotdiscretegroupsettings/
---
## PivotDiscreteGroupSettings class

Rappresenta il gruppo discreto del campo pivot.

```csharp
public class PivotDiscreteGroupSettings : PivotFieldGroupSettings
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DiscreteItems](../../aspose.cells.pivot/pivotdiscretegroupsettings/discreteitems/) { get; } | Ottiene gli elementi discreti. |
| [Items](../../aspose.cells.pivot/pivotdiscretegroupsettings/items/) { get; } | (**Obsolete.**) Ottiene gli elementi discreti. |
| override [Type](../../aspose.cells.pivot/pivotdiscretegroupsettings/type/) { get; } | Ottiene il tipo di gruppo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotDiscreteGroupSettingsDemo
    {
        public static void PivotDiscreteGroupSettingsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiunta di alcuni dati di esempio
            worksheet.Cells[0, 0].PutValue("Item");
            worksheet.Cells[0, 1].PutValue("Quantity");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(15);
            worksheet.Cells[3, 0].PutValue("A");
            worksheet.Cells[3, 1].PutValue(10);
            worksheet.Cells[4, 0].PutValue("B");
            worksheet.Cells[4, 1].PutValue(15);

            // Aggiungi una tabella pivot al foglio di lavoro
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Imposta i campi riga e dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Accesso al campo di riga
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1}) }, true);

            // Crea un'istanza di PivotDiscreteGroupSettings
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;

            // Imposta il tipo di gruppo su Discrete (Questa proprietà è di sola lettura)
            // Visualizza il tipo di gruppo corrente
            Console.WriteLine("Group Type: " + groupSettings.Type);

            // Salva la cartella di lavoro
            workbook.Save("PivotDiscreteGroupSettingsExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


