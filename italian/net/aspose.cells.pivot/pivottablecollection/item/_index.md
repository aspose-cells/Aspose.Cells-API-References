---
title: "PivotTableCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotTableCollection. Ottiene il report della PivotTable per indice"
type: docs
url: /it/net/aspose.cells.pivot/pivottablecollection/item/
---
## PivotTableCollection indexer (1 of 3)

Ottiene il report della PivotTable per indice.

```csharp
public PivotTable this[int index] { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file sorgente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla collezione di tabelle pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // Accedi alla prima tabella pivot usando la proprietà Item (indicizzatore)
            PivotTable pivotTable = pivotTables[0];
            
            // Calcola i dati della tabella pivot
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro modificata
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection indexer (2 of 3)

Ottiene il report della PivotTable per nome.

```csharp
public PivotTable this[string name] { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea dati di esempio
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(3000);

            // Aggiungi una tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Configura la tabella pivot usando la proprietà Item
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiorna e calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Accedi alla tabella pivot usando la proprietà Item
            PivotTable tableFromCollection = sheet.PivotTables["PivotTable1"];
            Console.WriteLine("Pivot table data source: " + string.Join(", ", tableFromCollection.DataSource));

            // Modifica i dati e aggiorna
            sheet.Cells["B2"].PutValue(1500);
            tableFromCollection.RefreshData();
            Console.WriteLine("Updated pivot table values");

            // Salva la cartella di lavoro
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection indexer (3 of 3)

Ottiene il [`PivotTable`](../../pivottable/) situato nella cella.

```csharp
public PivotTable this[int row, int column] { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 3000;

            try
            {
                // Aggiungi una tabella pivot al foglio di lavoro
                int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");

                // Accedi al PivotTableCollection
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Dimostra l'accesso a una tabella pivot utilizzando la proprietà Item (indicizzatore)
                PivotTable pivotTable = pivotTables[index];
                Console.WriteLine($"Accessed pivot table at index {index} with name: {pivotTable.Name}");

                // Dimostra l'accesso per nome utilizzando la proprietà Item
                PivotTable pivotTableByName = pivotTables["PivotTable1"];
                Console.WriteLine($"Accessed pivot table by name: {pivotTableByName.Name}");

                // Configura la tabella pivot
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

                // Aggiorna e calcola i dati
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Salva la cartella di lavoro
                workbook.Save("PivotTableItemDemo.xlsx");
                Console.WriteLine("Pivot table demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


