---
title: "PivotTableCollection.RemoveAt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTableCollection. Elimina la PivotTable all'indice specificato e cancella i dati della PivotTable"
type: docs
url: /it/net/aspose.cells.pivot/pivottablecollection/removeat/
---
## RemoveAt(int) {#removeat}

Elimina la PivotTable all'indice specificato e cancella i dati della PivotTable

```csharp
public void RemoveAt(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | l'indice di posizione nella raccolta PivotTable |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Aggiungi più tabelle pivot
            sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            sheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
            sheet.PivotTables.Add("A1:B4", "D20", "PivotTable3");

            // Rimuovi la tabella pivot all'indice 1 (seconda tabella pivot)
            sheet.PivotTables.RemoveAt(1);

            // Verifica il conteggio dopo la rimozione
            Console.WriteLine("Pivot Tables Count: " + sheet.PivotTables.Count);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, bool) {#removeat_2}

Elimina la PivotTable all'indice specificato

```csharp
public void RemoveAt(int index, bool keepData)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | l'indice di posizione nella raccolta PivotTable |
| keepData | Booleano | Indica se mantenere i dati della PivotTable |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveAtWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Aggiungi una tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "D9", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Dimostra RemoveAt con keepData=true
            worksheet.PivotTables.RemoveAt(0, true);
            Console.WriteLine("Pivot table removed with keepData=true. Cell D9 value: " + worksheet.Cells["D9"].Value);

            // Aggiungi un'altra tabella pivot
            index = worksheet.PivotTables.Add("A1:B4", "D9", "PivotTable2");
            pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Dimostra RemoveAt con keepData=false
            worksheet.PivotTables.RemoveAt(0, false);
            Console.WriteLine("Pivot table removed with keepData=false. Cell D9 value: " + worksheet.Cells["D9"].Value);
        }
    }
}
```

### Vedi anche

* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


