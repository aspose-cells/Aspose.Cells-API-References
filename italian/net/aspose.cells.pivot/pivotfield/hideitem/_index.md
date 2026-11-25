---
title: "PivotField.HideItem"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Imposta se lo specifico PivotItem in un campo dati è nascosto."
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/hideitem/
---
## HideItem(int, bool) {#hideitem}

Imposta se lo specifico PivotItem in un campo dati è nascosto.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(int index, bool isHidden)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | l'indice del pivotItem nel pivotField. |
| isHidden | Booleano | se il PivotItem specifico è nascosto |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.PivotItems[int].IsHidden. Questo metodo sarà rimosso 12 mesi dopo, a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideItemWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con una tabella pivot di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Dati di esempio per la tabella pivot
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("PO-23-05");
            sheet.Cells["A3"].PutValue("PO-23-06");
            sheet.Cells["A4"].PutValue("PO-23-05");
            sheet.Cells["A5"].PutValue("PO-23-07");
            
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(1500);
            sheet.Cells["B5"].PutValue(3000);

            // Crea tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Nascondi gli elementi che non sono "PO-23-05"
            for (int i = 0; i < pivotField.ItemCount; i++)
            {
                pivotField.HideItem(i, pivotField.Items[i] != "PO-23-05");
            }
            
            // Calcola tabella pivot
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldHideItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## HideItem(string, bool) {#hideitem_1}

Imposta se lo specifico PivotItem in un campo dati è nascosto.

```csharp
[Obsolete("Use PivotField.PivotItems[string].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideItem(string itemValue, bool isHidden)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| itemValue | String | Il nome del pivotItem nel pivotField. |
| isHidden | Booleano | Indica se il specifico PivotItem è nascosto |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare la proprietà PivotField.PivotItems[string].IsHidden. Questo metodo sarà rimosso 12 mesi dopo, a partire da agosto 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodHideItemWithStringBooleanDemo
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
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 5;

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");

            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Chiama il metodo HideItem con i parametri (String, Boolean)
                pivotField.HideItem("Apple", true);

                Console.WriteLine("Method executed successfully with parameters (String, Boolean)");
                Console.WriteLine("Apple items are now hidden in the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HideItem method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("PivotFieldMethodHideItemWithStringBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


