---
title: "PivotTable.GetSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Ottiene l'origine dati di questa tabella pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/getsource/
---
## GetSource() {#getsource}

Ottieni l'origine dati di questa tabella pivot.

```csharp
public string[] GetSource()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Crea tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ottieni e visualizza l'intervallo dei dati di origine
            string[] sourceData = pivotTable.GetSource();
            Console.WriteLine("Pivot Table Source: " + sourceData[0]);
            
            // Modifica l'origine dati
            pivotTable.ChangeDataSource(new[] { "A1:B4" });
            
            // Verifica l'origine modificata
            sourceData = pivotTable.GetSource();
            Console.WriteLine("Updated Pivot Table Source: " + sourceData[0]);
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## GetSource(bool) {#getsource_1}

Ottieni l'origine dati di questa tabella pivot.

```csharp
public string[] GetSource(bool isOriginal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isOriginal | Booleano | Indica se restituire l'origine dati originale o quella visualizzata. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetSourceWithBooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi alla prima tabella pivot
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Ottieni i dati di origine con percorso locale (true)
            string[] localSource = pivotTable.GetSource(true);
            Console.WriteLine("Local path source: " + localSource[0]);
            
            // Ottieni i dati di origine con percorso completo (false)
            string[] fullSource = pivotTable.GetSource(false);
            Console.WriteLine("Full path source: " + fullSource[0]);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


