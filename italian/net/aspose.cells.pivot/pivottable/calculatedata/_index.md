---
title: "PivotTable.CalculateData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Calcola i dati della tabella pivot nelle celle"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata_1}

Calcola i dati della PivotTable nelle celle.

```csharp
public void CalculateData()
```

### Osservazioni

Questo metodo calcola i dati solo con i dati memorizzati nella cache del [`PivotCache`](../pivotcache/). Quindi, se desideri calcolare con l'ultima fonte dati, utilizza il metodo [`Refresh`](../../pivotcache/refresh/). Se è stata modificata solo l'impostazione della tabella pivot, `CalculateData` è sufficiente.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            
            DateTime baseDate = new DateTime(2021, 11, 1);
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+2}"].PutValue(baseDate.AddDays(i));
                worksheet.Cells[$"B{i+2}"].PutValue(100 + i * 10);
            }

            // Crea tabella pivot - corretto garantendo parametri corretti
            int pivotIndex = worksheet.PivotTables.Add("A1:B16", "D3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campi alla pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Applica filtro data
            PivotField dateField = pivotTable.RowFields[0];
            dateField.FilterByDate(PivotFilterType.November, new DateTime(2021, 1, 1), new DateTime(2021, 12, 31));
            
            // Calcola i dati della pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata}

Calcola la tabella pivot con opzioni.

```csharp
public PivotTable[] CalculateData(PivotTableCalculateOption option)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| opzione | PivotTableCalculateOption | Le opzioni per calcolare la tabella pivot |

### Valore di ritorno

Restituisce tutte le tabelle pivot che sono state calcolate. Se [`RefreshData`](../../pivottablecalculateoption/refreshdata/) è true, tutte le tabelle pivot basate sulla stessa cache pivot verranno calcolate insieme.

### Osservazioni

Se [`RefreshData`](../../pivottablecalculateoption/refreshdata/) è true, questo metodo aggiornerà la cache pivot dalla fonte dati, quindi calcolerà tutte le tabelle pivot basate sulla stessa cache pivot. Altrimenti, verrà calcolato solo con i dati memorizzati nella cache pivot.

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataWithPivotTableCalculateOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Configura la tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Imposta le opzioni di calcolo
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                RefreshData = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calcola con opzioni
            pivotTable.CalculateData(options);

            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


