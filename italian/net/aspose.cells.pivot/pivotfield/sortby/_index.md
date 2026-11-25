---
title: "PivotField.SortBy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Ordina questo campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/sortby/
---
## SortBy(SortOrder) {#sortby}

Ordina questo campo pivot.

```csharp
public void SortBy(SortOrder sortType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sortType | SortOrder | Il tipo di ordinamento di questo campo. |

### Vedi anche

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int) {#sortby_1}

Ordina questo campo pivot.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method or PivotField.IsAutoSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sortType | SortOrder | Il tipo di ordinamento di questo campo. |
| fieldSortedBy | Int32 | L'indice del campo pivot per cui è ordinato. -1 indica l'ordinamento per le etichette dei dati di questo campo, altri valori indicano l'indice del campo dati per cui è ordinato. |

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotField.SortBy(SortOrder, int,string) o la proprietà PivotField.IsAutoSort. Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Country");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("USA");
            worksheet.Cells["A3"].PutValue("UK");
            worksheet.Cells["A4"].PutValue("Germany");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(1500);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga
            int rowIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[rowIndex];
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ordina il campo di riga in ordine discendente con indice -1
            rowField.SortBy(SortOrder.Descending, -1);
            
            // Aggiorna e calcola la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, PivotLineType, string) {#sortby_2}

Ordina questo campo pivot.

```csharp
[Obsolete("Use PivotField.SortBy(SortOrder, int,string) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SortBy(SortOrder sortType, int fieldSortedBy, PivotLineType dataType, string cellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sortType | SortOrder | Il tipo di ordinamento di questo campo. |
| fieldSortedBy | Int32 | L'indice del campo pivot per cui è ordinato. -1 indica l'ordinamento per le etichette dei dati di questo campo, altri valori indicano l'indice del campo dati per cui è ordinato. |
| dataType | PivotLineType | Il tipo di dati per cui è ordinato. |
| cellName | String | Ordina per valori nella riga o nella colonna |

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare il metodo PivotField.SortBy(SortOrder, int,string). Questo metodo sarà rimosso 12 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodSortByWithSortOrderInt32PivotLineTypeStrDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("B");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);
            worksheet.Cells["B4"].PutValue(100);

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ordina il campo di riga
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.Regular, "E4");
            
            // Calcola i dati
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldSortByDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SortOrder](../../../aspose.cells/sortorder/)
* enum [PivotLineType](../../pivotlinetype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SortBy(SortOrder, int, string) {#sortby_3}

Ordina questo campo pivot.

```csharp
public void SortBy(SortOrder sortType, int fieldSortedBy, string cellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sortType | SortOrder | Il tipo di ordinamento di questo campo. |
| fieldSortedBy | Int32 | L'indice del campo pivot per cui è ordinato. -1 indica l'ordinamento per le etichette dei dati di questo campo, altri valori indicano l'indice del campo dati per cui è ordinato. |
| cellName | String | Ordina per valori nella riga o nella colonna. Se Null, raggruppa per il totale del campo, altrimenti raggruppa per i valori nella colonna o riga selezionata. |

### Vedi anche

* enum [SortOrder](../../../aspose.cells/sortorder/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


