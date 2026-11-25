---
title: "PivotTable.EnableDataValueEditing"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTable. Specifica un valore booleano che indica se all'utente è consentito modificare le celle nell'area dati della tabella pivot. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/enabledatavalueediting/
---
## PivotTable.EnableDataValueEditing property

Specifica un valore booleano che indica se all'utente è consentito modificare le celle nell'area dati della PivotTable. Il valore predefinito è false.

```csharp
public bool EnableDataValueEditing { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyEnableDataValueEditingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Bike");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Car");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Bike");
            worksheet.Cells["B4"].PutValue(1500);
            worksheet.Cells["A5"].PutValue("Car");
            worksheet.Cells["B5"].PutValue(3000);

            // Aggiungi una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campo riga e campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Visualizza il valore corrente di EnableDataValueEditing
            Console.WriteLine("Current EnableDataValueEditing value: " + pivotTable.EnableDataValueEditing);

            // Abilita la modifica dei valori dei dati
            pivotTable.EnableDataValueEditing = true;

            // Calcola i dati per popolare la tabella pivot
            pivotTable.CalculateData();

            // Salva la cartella di lavoro prima della modifica
            workbook.Save("PivotTableBeforeEdit.xlsx");

            // Ora possiamo modificare i valori dei dati direttamente nella tabella pivot
            // Per dimostrazione, modificheremo una cella nell'area dati
            Cell dataCell = worksheet.Cells["F5"]; // Assuming this is a data cell
            if (dataCell != null)
            {
                dataCell.PutValue(2500); // Modify the value
            }

            // Salva la cartella di lavoro dopo la modifica
            workbook.Save("PivotTableAfterEdit.xlsx");

            // Disabilita la modifica dei valori dei dati
            pivotTable.EnableDataValueEditing = false;
            Console.WriteLine("EnableDataValueEditing set to: " + pivotTable.EnableDataValueEditing);
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


