---
title: "TimelineCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo TimelineCollection. Aggiunge una nuova Timeline usando PivotTable come origine dati"
type: docs
url: /it/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Aggiungi una nuova Timeline utilizzando la PivotTable come origine dati

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto PivotTable |
| riga | Int32 | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo Timeline. |
| colonna | Int32 | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo Timeline. |
| baseFieldName | String | Il nome di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta della Timeline

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 1, 3);
            cells["C4"].Value = 200;

            // Crea tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Column, 1);
            pivot.AddFieldToArea(PivotFieldType.Data, 2);

            // Aggiungi timeline collegata alla tabella pivot
            sheet.Timelines.Add(pivot, 10, 5, "Date");
            
            // Salva cartella di lavoro
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Aggiungi una nuova Timeline utilizzando la PivotTable come origine dati

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto PivotTable |
| destCellName | String | Il nome della cella nell'angolo in alto a sinistra dell'intervallo Timeline. |
| baseFieldName | String | Il nome di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta della Timeline

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(DateTime.Now);
            sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            
            // Aggiungi tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "C1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Aggiungi timeline collegata alla tabella pivot
            sheet.Timelines.Add(pivot, "E1", "Date");
            
            // Salva la cartella di lavoro
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Aggiungi una nuova Timeline utilizzando la PivotTable come origine dati

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto PivotTable |
| riga | Int32 | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo Timeline. |
| colonna | Int32 | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo Timeline. |
| baseFieldIndex | Int32 | L'indice di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta della Timeline

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;

            // Aggiungi tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi controllo timeline
            sheet.Timelines.Add(pivot, 15, 5, 1);
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Aggiungi una nuova Timeline utilizzando la PivotTable come origine dati

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto PivotTable |
| destCellName | String | Il nome della cella nell'angolo in alto a sinistra dell'intervallo Timeline. |
| baseFieldIndex | Int32 | L'indice di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta della Timeline

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Date");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            cells["A2"].PutValue(new DateTime(2023, 1, 1));
            cells["B2"].PutValue("A");
            cells["C2"].PutValue(100);
            
            cells["A3"].PutValue(new DateTime(2023, 1, 2));
            cells["B3"].PutValue("B");
            cells["C3"].PutValue(200);
            
            cells["A4"].PutValue(new DateTime(2023, 1, 3));
            cells["B4"].PutValue("A");
            cells["C4"].PutValue(150);

            // Crea tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Aggiorna i dati della tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Trova l'indice del campo base per il campo "Date"
            int dateFieldIndex = -1;
            for (int i = 0; i < pivotTable.BaseFields.Count; i++)
            {
                if (pivotTable.BaseFields[i].Name == "Date")
                {
                    dateFieldIndex = i;
                    break;
                }
            }

            // Aggiungi timeline usando l'indice trovato
            if (dateFieldIndex >= 0)
            {
                sheet.Timelines.Add(pivotTable, "H2", dateFieldIndex);
            }

            // Salva il risultato
            workbook.Save("TimelineCollectionMethodAddWithPivotTableStringInt32Demo_output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Aggiungi una nuova Timeline utilizzando la PivotTable come origine dati

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto PivotTable |
| riga | Int32 | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo Timeline. |
| colonna | Int32 | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo Timeline. |
| baseField | PivotField | Il PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta della Timeline

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Date";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "P1";
            cells["B2"].Value = new DateTime(2023, 1, 1);
            cells["C2"].Value = 100;
            
            cells["A3"].Value = "P2";
            cells["B3"].Value = new DateTime(2023, 1, 2);
            cells["C3"].Value = 150;
            
            cells["A4"].Value = "P1";
            cells["B4"].Value = new DateTime(2023, 2, 1);
            cells["C4"].Value = 200;

            // Crea tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            
            // Aggiungi campi pivot
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);
            pivot.AddFieldToArea(PivotFieldType.Column, pivot.BaseFields[1]);
            pivot.AddFieldToArea(PivotFieldType.Data, pivot.BaseFields[2]);

            // Aggiungi timeline usando la tabella pivot
            sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
            
            // Salva la cartella di lavoro
            workbook.Save("TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Aggiungi una nuova Timeline utilizzando la PivotTable come origine dati

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto PivotTable |
| destCellName | String | Il nome della cella nell'angolo in alto a sinistra dell'intervallo Timeline. |
| baseField | PivotField | Il PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta della Timeline

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class TimelineCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;

            // Crea tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivot.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Aggiungi timeline usando la tabella pivot come origine dati
            sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[0]);
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


