---
title: "PivotFieldSortSetting.IsSortByLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFieldSortSetting. Indica se ordinare il campo per se stesso o per il campo dati"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldsortsetting/issortbylabels/
---
## PivotFieldSortSetting.IsSortByLabels property

Indica se ordinare il campo per se stesso o per il campo dati.

```csharp
public bool IsSortByLabels { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSortSettingPropertyIsSortByLabelsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            var cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Ottieni l'impostazione di ordinamento del campo pivot
            PivotField pivotField = pivotTable.RowFields[0];
            PivotFieldSortSetting sortSetting = pivotField.SortSetting;

            // Visualizza valore corrente di IsSortByLabels
            Console.WriteLine("Current IsSortByLabels value: " + sortSetting.IsSortByLabels);

            // Nota: IsSortByLabels è di sola lettura, quindi non possiamo impostarlo direttamente
            // Invece, dimostreremo il suo significato esaminando le impostazioni di ordinamento

            // Mostra le proprietà di ordinamento correlate
            Console.WriteLine("SortType: " + sortSetting.SortType);
            Console.WriteLine("FieldIndex: " + sortSetting.FieldIndex);
            Console.WriteLine("IsSimpleSort: " + sortSetting.IsSimpleSort);

            // Salva la cartella di lavoro
            workbook.Save("PivotFieldSortSettingPropertyIsSortByLabelsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


