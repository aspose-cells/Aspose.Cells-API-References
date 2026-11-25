---
title: "PivotTable.AddCalculatedField"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Aggiunge un campo calcolato al campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/addcalculatedfield/
---
## AddCalculatedField(string, string, bool) {#addcalculatedfield_1}

Aggiunge un campo calcolato al campo pivot.

```csharp
public void AddCalculatedField(string name, string formula, bool dragToDataArea)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome del campo calcolato |
| formula | String | La formula del campo calcolato. |
| dragToDataArea | Booleano | True, trascina immediatamente questo campo nell'area dati |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddCalculatedFieldWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "A";
            cells["B2"].Value = 100;
            cells["A3"].Value = "B";
            cells["B3"].Value = 150;
            cells["A4"].Value = "C";
            cells["B4"].Value = 200;

            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Aggiungi campo calcolato
            pivotTable.AddCalculatedField("DoubleSales", "=Sales*2", true);

            // Salva la cartella di lavoro
            workbook.Save("PivotTableWithCalculatedField.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddCalculatedField(string, string) {#addcalculatedfield}

Aggiunge un campo calcolato al campo pivot e lo trascina nell'area dati.

```csharp
public void AddCalculatedField(string name, string formula)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome del campo calcolato |
| formula | String | La formula del campo calcolato. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddCalculatedFieldWithStringStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(8);
            
            worksheet.Cells["C1"].PutValue("Quantity");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(3);
            worksheet.Cells["C4"].PutValue(10);

            // Crea collezione di tabelle pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Aggiungi una tabella pivot e ottieni il suo indice
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            
            // Ottieni l'oggetto della tabella pivot
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Aggiungi campi all'area delle righe
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Aggiungi campi dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Aggiungi campo calcolato
            pivotTable.AddCalculatedField("Total", "=Price*Quantity");
            
            // Formatta il campo dati
            pivotTable.DataFields["Total"].NumberFormat = "$#,##0.00";
            
            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableWithCalculatedField.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


