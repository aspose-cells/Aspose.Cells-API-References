---
title: "PivotField.GroupBy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Raggruppa automaticamente il campo con intervallo"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/groupby/
---
## GroupBy(double, bool) {#groupby_7}

Raggruppa automaticamente il campo con intervallo

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(double interval, bool newField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| intervallo | Double | L'interno del gruppo. Il valore automatico verrà assegnato se è zero, |
| newField | Booleano | Indica se aggiungere un nuovo campo alla tabella pivot. Solo per il raggruppamento DateTime. |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions). Questo metodo sarà rimosso 6 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla prima tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Aggiungi campo all'area colonne
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 2);
            
            // Raggruppa il campo per 1 (intervallo) con intervallo automatico
            pivotTable.BaseFields[2].GroupBy(1.0, true);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(PivotGroupByType[], double, bool) {#groupby_6}

Raggruppa automaticamente il campo con interno

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void GroupBy(PivotGroupByType[] groups, double interval, bool newField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| gruppi | PivotGroupByType[] | Tipi di raggruppamento |
| intervallo | Double | L'interno del gruppo. Il valore automatico verrà assegnato se è zero, funziona solo per il raggruppamento per Numeri o Giorni. |
| newField | Booleano | Indica se aggiungere un nuovo campo alla tabella pivot. |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions). Questo metodo sarà rimosso 6 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Vedi anche

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DateTime, DateTime, PivotGroupByType[], double, bool) {#groupby_5}

Raggruppa il file per i tipi di gruppo data.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DateTime start, DateTime end, PivotGroupByType[] groups, double interval, 
    bool firstAsNewField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | DateTime | La data e ora di inizio |
| fine | DateTime | La data e ora di fine |
| gruppi | PivotGroupByType[] | Tipi di raggruppamento |
| intervallo | Double | L'intervallo |
| firstAsNewField | Booleano | Indica se aggiungere un nuovo campo alla tabella pivot. Solo per il primo elemento del gruppo. |

### Valore di ritorno

False indica che questo campo non può essere raggruppato per data e ora.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions). Questo metodo sarà rimosso 6 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithDateTimeDateTimePivotGroupByTyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con date per la tabella pivot
            worksheet.Cells["A1"].Value = "Date";
            worksheet.Cells["A2"].Value = new DateTime(2023, 1, 15);
            worksheet.Cells["A3"].Value = new DateTime(2023, 2, 20);
            worksheet.Cells["A4"].Value = new DateTime(2023, 3, 10);
            worksheet.Cells["A5"].Value = new DateTime(2023, 4, 5);
            worksheet.Cells["A6"].Value = new DateTime(2023, 5, 25);
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1500;
            worksheet.Cells["B3"].Value = 2300;
            worksheet.Cells["B4"].Value = 3200;
            worksheet.Cells["B5"].Value = 4100;
            worksheet.Cells["B6"].Value = 5000;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields[0];

            // Prepara i parametri per il metodo GroupBy
            DateTime startDate = new DateTime(2023, 1, 1);
            DateTime endDate = new DateTime(2023, 6, 30);
            PivotGroupByType[] groupTypes = new PivotGroupByType[] { PivotGroupByType.Months };
            double interval = 1;
            bool firstAsNewField = false;

            try
            {
                // Chiama il metodo GroupBy con parametri data
                bool result = pivotField.GroupBy(startDate, endDate, groupTypes, interval, firstAsNewField);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Aggiorna la tabella pivot
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldGroupByDateTimeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, DateTime, bool, DateTime, PivotGroupByType[], double, bool) {#groupby_3}

Raggruppa il file per i tipi di gruppo data.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, DateTime start, bool isAutoEnd, DateTime end, 
    PivotGroupByType[] groups, double interval, bool firstAsNewField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isAutoStart | Booleano | Indica se rilevare automaticamente il valore della data e ora di inizio. |
| inizio | DateTime | La data e ora di inizio |
| isAutoEnd | Booleano | Indica se rilevare automaticamente il valore della data e ora di fine. |
| fine | DateTime | La data e ora di fine |
| gruppi | PivotGroupByType[] | Tipi di raggruppamento |
| intervallo | Double | L'intervallo |
| firstAsNewField | Booleano | Indica se aggiungere un nuovo campo alla tabella pivot. Solo per il primo elemento del gruppo. |

### Valore di ritorno

False indica che questo campo non può essere raggruppato per data e ora.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions). Questo metodo sarà rimosso 6 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Vedi anche

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(double, double, double, bool) {#groupby_4}

Raggruppa il file per numero.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(double start, double end, double interval, bool newField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| inizio | Double | Il valore di inizio |
| fine | Double | Il valore di fine |
| intervallo | Double | L'intervallo |
| newField | Booleano | Indica se aggiungere un nuovo campo alla tabella pivot |

### Valore di ritorno

False indica che questo campo non può essere raggruppato per data e ora.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions). Questo metodo sarà rimosso 6 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGroupByWithDoubleDoubleDoubleBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Value";
            worksheet.Cells["A2"].Value = 1;
            worksheet.Cells["A3"].Value = 2;
            worksheet.Cells["A4"].Value = 3;
            worksheet.Cells["A5"].Value = 4;
            worksheet.Cells["A6"].Value = 5;
            worksheet.Cells["A7"].Value = 6;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:A7", "D1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga e raggruppalo
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.GroupBy(1, 6, 2, false); // Group values from 1 to 6 with interval 2, auto range false
            
            // Salva la cartella di lavoro
            workbook.Save("PivotGroupByExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(bool, double, bool, double, double, bool) {#groupby_2}

Raggruppa il file per numero.

```csharp
[Obsolete("Use PivotField.GroupBy(PivotFieldGroupOptions) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(bool isAutoStart, double start, bool isAutoEnd, double end, double interval, 
    bool newField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isAutoStart | Booleano | Indica se rilevare automaticamente il valore di inizio. |
| inizio | Double | Il valore di inizio |
| isAutoEnd | Booleano | Indica se rilevare automaticamente il valore di fine. |
| fine | Double | Il valore di fine |
| intervallo | Double | L'intervallo |
| newField | Booleano | Indica se aggiungere un nuovo campo alla tabella pivot |

### Valore di ritorno

False indica che questo campo non può essere raggruppato per data e ora.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions). Questo metodo sarà rimosso 6 mesi dopo, a partire da settembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Vedi anche

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(CustomPiovtFieldGroupItem[], bool) {#groupby}

Raggruppa il campo in modo personalizzato.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(CustomPiovtFieldGroupItem[] customGroupItems, bool newField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| customGroupItems | CustomPiovtFieldGroupItem[] | Gli elementi del gruppo personalizzato. |
| newField | Booleano | Indica se aggiungere un nuovo campo alla tabella pivot |

### Valore di ritorno

False indica che questo campo non può essere raggruppato per data e ora.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions options) con la proprietà PivotFieldGroupOptions.DiscreteGroupItems. Questo metodo sarà rimosso tra 6 mesi a partire da luglio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodGroupByWithCustomPiovtFieldGroupItemBooDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Grapes";
            worksheet.Cells["A6"].Value = "Mango";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;
            worksheet.Cells["B5"].Value = 4000;
            worksheet.Cells["B6"].Value = 5000;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Ottieni il campo pivot
            PivotField pivotField = pivotTable.RowFields[0];

            // Crea elementi di gruppo personalizzati
            CustomPiovtFieldGroupItem[] customGroupItems = new CustomPiovtFieldGroupItem[2];
            customGroupItems[0] = new CustomPiovtFieldGroupItem("Group1", new int[] { 0, 1 }); // Apple (index 0), Banana (index 1)
            customGroupItems[1] = new CustomPiovtFieldGroupItem("Group2", new int[] { 2, 3, 4 }); // Orange (2), Grapes (3), Mango (4)

            try
            {
                // Chiama il metodo GroupBy con elementi di gruppo personalizzati
                bool result = pivotField.GroupBy(customGroupItems, false);
                
                Console.WriteLine("GroupBy method executed successfully. Result: " + result);
                
                // Aggiorna la tabella pivot
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GroupBy method: {ex.Message}");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFieldGroupByCustomDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CustomPiovtFieldGroupItem](../../custompiovtfieldgroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GroupBy(DiscreteGroupItem[], bool) {#groupby_1}

Raggruppa il campo in modo personalizzato.

```csharp
[Obsolete("Use PivotField.Group(PivotFieldGroupOptions options) method with PivotFieldGroupOptions.DiscreteGroupItems property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool GroupBy(DiscreteGroupItem[] customGroupItems, bool newField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| customGroupItems | DiscreteGroupItem[] | Gli elementi del gruppo personalizzato. |
| newField | Booleano | Indica se aggiungere un nuovo campo alla tabella pivot |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotField.Group(PivotFieldGroupOptions options) con la proprietà PivotFieldGroupOptions.DiscreteGroupItems. Questo metodo sarà rimosso tra 6 mesi a partire da luglio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Vedi anche

* class [DiscreteGroupItem](../../discretegroupitem/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


