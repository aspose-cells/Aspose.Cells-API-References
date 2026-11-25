---
title: "PivotFieldSortSetting.IsSimpleSort"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFieldSortSetting. Indica se verrà applicata un'operazione di ordinamento dati semplice"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldsortsetting/issimplesort/
---
## PivotFieldSortSetting.IsSimpleSort property

Indica se verrà applicata un'operazione di ordinamento dati semplice.

```csharp
public bool IsSimpleSort { get; set; }
```

### Osservazioni

Il valore predefinito è true.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSimpleSortDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;
            worksheet.Cells["B5"].Value = 150;
            worksheet.Cells["B6"].Value = 250;

            // Crea una tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields[0];

            // Ottieni impostazione di ordinamento (proprietà di sola lettura)
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // Visualizza valore corrente di IsSimpleSort
            Console.WriteLine("Current IsSimpleSort value: " + sortSetting.IsSimpleSort);

            // Nota: IsSimpleSort è di sola lettura, quindi non possiamo impostarlo direttamente
            // Per dimostrare l'ordinamento, creeremo una nuova tabella pivot con un ordinamento diverso

            // Crea un'altra tabella pivot con ordinamento personalizzato
            pivotIndex = pivotTables.Add("A1:B6", "E3", "PivotTable2");
            PivotTable pivotTable2 = pivotTables[pivotIndex];
            pivotTable2.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable2.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ordina il campo pivot utilizzando il metodo disponibile
            PivotField pivotField2 = pivotTable2.RowFields[0];
            pivotField2.SortBy(SortOrder.Ascending, -1);

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldSortSettingPropertyIsSimpleSortDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


