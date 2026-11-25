---
title: "PivotFieldCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFieldCollection. Ottiene l'oggetto PivotField Object all'indice specifico"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldcollection/item/
---
## PivotFieldCollection indexer (1 of 2)

Ottiene l'oggetto PivotField Object all'indice specifico.

```csharp
public PivotField this[int index] { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e ottieni il primo foglio
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Aggiungi una tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campi alle aree
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Accedi al primo campo di riga usando la proprietà Item e imposta IsAutoSort
            pivotTable.RowFields[0].IsAutoSort = true;
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotFieldCollection indexer (2 of 2)

Ottiene l'oggetto PivotField Object del nome specifico.

```csharp
public PivotField this[string name] { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            ws.Cells["A1"].Value = "Category";
            ws.Cells["B1"].Value = "Value";
            ws.Cells["A2"].Value = "A";
            ws.Cells["B2"].Value = 10;
            ws.Cells["A3"].Value = "B";
            ws.Cells["B3"].Value = 20;
            ws.Cells["A4"].Value = "A";
            ws.Cells["B4"].Value = 30;
            ws.Cells["A5"].Value = "B";
            ws.Cells["B5"].Value = 40;

            // Crea tabella pivot
            int index = ws.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pTable = ws.PivotTables[index];
            
            // Aggiungi campi alla tabella pivot
            pTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Dimostra l'uso della proprietà Item
            pTable.DataFields["Sum of Value"].IsAutoSort = true;
            pTable.DataFields["Sum of Value"].IsAscendSort = false;
            
            // Aggiorna e calcola la tabella pivot
            pTable.RefreshData();
            pTable.CalculateData();
            
            // Salva la cartella di lavoro
            wb.Save("PivotFieldCollectionPropertyItemDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


