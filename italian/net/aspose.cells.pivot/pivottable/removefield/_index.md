---
title: "PivotTable.RemoveField"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Rimuove un campo da un'area di campo specifica"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/removefield/
---
## RemoveField(PivotFieldType, string) {#removefield_2}

Rimuove un campo da un'area di campo specifica

```csharp
public void RemoveField(PivotFieldType fieldType, string fieldName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | PivotFieldType | Il tipo di area dei campi. |
| fieldName | String | Il nome nei campi base. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla prima tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Rimuovi il campo "c" dall'area Dati
            pivotTable.RemoveField(PivotFieldType.Data, "c");
            
            // Calcola i dati della tabella pivot
            pivotTable.CalculateData();
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, int) {#removefield_1}

Rimuove un campo da una specifica regione pivot.

```csharp
public void RemoveField(PivotFieldType fieldType, int baseFieldIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | PivotFieldType | Il tipo di area dei campi. |
| baseFieldIndex | Int32 | L'indice del campo nei campi base. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodRemoveFieldWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Crea una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            try
            {
                // Rimuovi il campo riga (indice 0) dalla tabella pivot
                pivotTable.RemoveField(PivotFieldType.Row, 0);
                
                Console.WriteLine("Row field removed successfully from the pivot table");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveField method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("PivotTableRemoveFieldDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RemoveField(PivotFieldType, PivotField) {#removefield}

Rimuovi il campo da una specifica area di campo

```csharp
public void RemoveField(PivotFieldType fieldType, PivotField pivotField)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | PivotFieldType | il tipo di area dei campi. |
| pivotField | PivotField | il campo nei campi base. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRemoveFieldWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("TestFile.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla prima tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Rimuovi un campo colonna dalla tabella pivot
            if (pivotTable.ColumnFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Column, pivotTable.ColumnFields[0]);
            }
            
            // Rimuovi un campo dati dalla tabella pivot
            if (pivotTable.DataFields.Count > 0)
            {
                pivotTable.RemoveField(PivotFieldType.Data, pivotTable.DataFields[0]);
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ModifiedPivotTable.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


