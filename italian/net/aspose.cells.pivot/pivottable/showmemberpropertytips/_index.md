---
title: "PivotTable.ShowMemberPropertyTips"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Specifica un valore booleano che indica se le informazioni sulla proprietà del membro devono essere omesse dai tooltip della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showmemberpropertytips/
---
## PivotTable.ShowMemberPropertyTips property

Specifica un valore booleano che indica se le informazioni delle proprietà dei membri devono essere omesse dai suggerimenti della PivotTable.

```csharp
public bool ShowMemberPropertyTips { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowMemberPropertyTipsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["B5"].PutValue(2500);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visualizza il valore corrente di ShowMemberPropertyTips
            Console.WriteLine("Current ShowMemberPropertyTips value: " + pivotTable.ShowMemberPropertyTips);

            // Modifica la proprietà ShowMemberPropertyTips
            pivotTable.ShowMemberPropertyTips = false;
            Console.WriteLine("ShowMemberPropertyTips set to: " + pivotTable.ShowMemberPropertyTips);

            // Calcola i dati e aggiorna la tabella pivot
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Salva la cartella di lavoro
            workbook.Save("PivotTablePropertyShowMemberPropertyTipsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


