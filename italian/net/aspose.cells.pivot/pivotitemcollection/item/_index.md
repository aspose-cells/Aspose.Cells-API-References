---
title: "PivotItemCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotItemCollection. Restituisce l'oggetto PivotItem all'indice specificato"
type: docs
url: /it/net/aspose.cells.pivot/pivotitemcollection/item/
---
## PivotItemCollection indexer (1 of 2)

Restituisce l'oggetto PivotItem all'indice specificato.

```csharp
public PivotItem this[int index] { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 150;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 200;
            
            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Accedi agli elementi pivot usando la proprietà Item
            PivotItemCollection pivotItems = pivotTable.RowFields[0].PivotItems;
            
            // Dimostra l'uso della proprietà Item
            Console.WriteLine("First pivot item: " + pivotItems[0].Name);
            Console.WriteLine("Second pivot item: " + pivotItems[1].Name);
            Console.WriteLine("Third pivot item: " + pivotItems[2].Name);
        }
    }
}
```

### Vedi anche

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotItemCollection indexer (2 of 2)

Restituisce il [`PivotItem`](../../pivotitem/) per il nome specifico.

```csharp
public PivotItem this[string itemValue] { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("PivotTest3.xlsx");
            
            // Aggiungi un nuovo foglio di lavoro per la tabella pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            Worksheet dataSheet = workbook.Worksheets["New Hardware - Yearly"];

            // Aggiungi tabella pivot
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "PivotTable");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "2014");

            // Configura la tabella pivot
            pivotTable.RowFields["Vendor"].SetSubtotals(PivotFieldSubtotalType.None, true);
            pivotTable.ShowColumnGrandTotals = false;

            // Aggiorna e calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Dimostra l'uso della proprietà Item e le operazioni di spostamento
            PivotItemCollection items = pivotTable.RowFields["Item"].PivotItems;
            
            // Accedi agli elementi usando la proprietà Item
            items["4H12"].Move(0, true);
            items["DIF400"].Move(-1, true);
            
            pivotTable.CalculateData();
            
            items["CA32"].Move(0, true);
            items["AAA3"].Move(-1, true);

            // Salva la cartella di lavoro
            workbook.Save("PivotItemCollectionDemo_Output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


