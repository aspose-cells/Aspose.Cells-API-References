---
title: "SlicerCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SlicerCollection. Aggiungi un nuovo Slicer usando PivotTable come origine dati"
type: docs
url: /it/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Aggiungi un nuovo Slicer utilizzando PivotTable come origine dati

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto PivotTable |
| destCellName | String | La cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| baseFieldName | String | Il nome di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta del Slicer

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];

            // Aggiungi slicer
            int slicerIndex = worksheet.Slicers.Add(pivot, "E3", "fruit");
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Aggiungi un nuovo Slicer utilizzando PivotTable come origine dati

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto PivotTable |
| riga | Int32 | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| colonna | Int32 | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| baseFieldName | String | Il nome di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta del Slicer

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea dati di esempio
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Fruit");
            cells["B1"].PutValue("Quantity");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(50);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(30);

            // Crea tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi slicer
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivotTable, 20, 12, "fruit");

            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Aggiungi un nuovo Slicer utilizzando PivotTable come origine dati

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto PivotTable |
| riga | Int32 | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| colonna | Int32 | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| baseFieldIndex | Int32 | L'indice di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta del Slicer

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Aggiungi tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = worksheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi slicer per la tabella pivot
            int slicerIndex = worksheet.Slicers.Add(pivot, 20, 8, 0);
            Slicer slicer = worksheet.Slicers[slicerIndex];
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Aggiungi un nuovo Slicer utilizzando PivotTable come origine dati

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto PivotTable |
| destCellName | String | La cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| baseFieldIndex | Int32 | L'indice di PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta del Slicer

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringInt32Demo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 20;

            // Crea tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Aggiungi slicer
            SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "A1", 0);
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Aggiungi un nuovo Slicer utilizzando PivotTable come origine dati

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto PivotTable |
| riga | Int32 | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| colonna | Int32 | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| baseField | PivotField | Il PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta del Slicer

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 5;
            cells["B3"].Value = 3;
            cells["B4"].Value = 7;

            // Crea tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];

            // Aggiungi campi pivot
            pivot.AddFieldToArea(PivotFieldType.Row, 0);
            pivot.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi slicer
            int slicerIndex = sheet.Slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Salva la cartella di lavoro
            workbook.Save("SlicerCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Aggiungi un nuovo Slicer utilizzando PivotTable come origine dati

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivot | PivotTable | Oggetto PivotTable |
| destCellName | String | La cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| baseField | PivotField | Il PivotField in PivotTable.BaseFields |

### Valore di ritorno

Il nuovo indice di aggiunta del Slicer

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B1"].Value = "Quantity";
            cells["B2"].Value = 10;
            cells["B3"].Value = 20;
            cells["B4"].Value = 30;

            // Crea tabella pivot
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivot = pivotTables[index];
            pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);

            // Aggiungi slicer
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(pivot, "I3", pivot.BaseFields[0]);

            // Salva la cartella di lavoro
            workbook.Save("SlicerCollectionMethodAddWithPivotTableStringPivotFieldDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Aggiungi un nuovo Slicer usando ListObjet come origine dati

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tabella | ListObject | oggetto ListObject |
| indice | Int32 | L'indice di ListColumn in ListObject.ListColumns |
| destCellName | String | La cella nell'angolo in alto a sinistra dell'intervallo Slicer. |

### Valore di ritorno

Il nuovo indice di aggiunta del Slicer

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea dati di esempio e oggetto lista
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue("E38");
            worksheet.Cells["A3"].PutValue("E39");
            worksheet.Cells["A4"].PutValue("E40");
            
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 0, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // Aggiungi slicer per l'oggetto lista - nota: Slicers.Add restituisce un indice int
            int slicerIndex = worksheet.Slicers.Add(listObject, 0, "E38");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            
            // Salva la cartella di lavoro
            workbook.Save("SlicerCollectionMethodAddWithListObjectInt32StringDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Aggiungi un nuovo Slicer usando ListObjet come origine dati

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tabella | ListObject | oggetto ListObject |
| listColumn | ListColumn | Il ListColumn in ListObject.ListColumns |
| destCellName | String | La cella nell'angolo in alto a sinistra dell'intervallo Slicer. |

### Valore di ritorno

Il nuovo indice di aggiunta del Slicer

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["A3"].PutValue("Data3");
            worksheet.Cells["B3"].PutValue("Data4");

            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];

            SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(table, table.ListColumns[1], "I38");

            worksheet.Cells.SetColumnWidth(0, 20);
            worksheet.Cells.SetColumnWidth(1, 20);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Aggiungi un nuovo Slicer usando ListObjet come origine dati

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tabella | ListObject | oggetto ListObject |
| listColumn | ListColumn | Il ListColumn in ListObject.ListColumns |
| riga | Int32 | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |
| colonna | Int32 | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo Slicer. |

### Valore di ritorno

Il nuovo indice di aggiunta del Slicer

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodAddWithListObjectListColumnInt32Int32Demo
    {
        public static void Run()
        {
            // Crea cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue("CatA");
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue("CatB");
            sheet.Cells["A4"].PutValue("Item3");
            sheet.Cells["B4"].PutValue("CatA");
            
            // Crea intervallo tabella
            int endRow = 4;
            string startCell = "A1";
            string endCell = $"B{endRow}";
            
            // Aggiungi tabella al foglio di lavoro usando il sovraccarico corretto
            int tableIndex = sheet.ListObjects.Add(startCell, endCell, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium2;
            
            // Aggiungi slicer per la colonna Categoria nella posizione (riga 6, colonna 1)
            Aspose.Cells.Slicers.SlicerCollection slicers = sheet.Slicers;
            slicers.Add(table, table.ListColumns[1], 6, 1);
            
            // Salva il risultato
            workbook.Save("SlicerOutput.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [ListColumn](../../../aspose.cells.tables/listcolumn/)
* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


