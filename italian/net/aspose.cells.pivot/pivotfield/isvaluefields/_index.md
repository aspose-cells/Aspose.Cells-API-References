---
title: "PivotField.IsValueFields"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotField. Indica se questo campo rappresenta campi valori"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/isvaluefields/
---
## PivotField.IsValueFields property

Indica se questo campo rappresenta campi valori.

```csharp
[Obsolete("Use PivotField.IsValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsValueFields { get; }
```

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.IsValuesField. Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldPropertyIsValueFieldsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Bike";
            worksheet.Cells["A4"].Value = "Car";
            worksheet.Cells["A5"].Value = "Car";
            worksheet.Cells["B2"].Value = "East";
            worksheet.Cells["B3"].Value = "West";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["B5"].Value = "West";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 3000;
            worksheet.Cells["C5"].Value = 4000;

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("=A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Aggiungi campo colonna
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");

            // Aggiungi un campo dati e ottienilo dalla collezione DataFields
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];

            // Visualizza il valore della proprietà IsValueFields
            Console.WriteLine("IsValueFields for data field: " + dataField.IsValueFields);

            // Prova a trovare un campo non dati per mostrare che IsValueFields è false
            foreach (PivotField field in pivotTable.RowFields)
            {
                Console.WriteLine("IsValueFields for row field '" + field.Name + "': " + field.IsValueFields);
            }

            // Salva il risultato
            workbook.Save("PivotFieldPropertyIsValueFieldsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


