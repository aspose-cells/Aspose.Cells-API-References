---
title: "PivotField.FilterTop10"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotField. Filtra per valori del campo pivot dei dati"
type: docs
url: /it/net/aspose.cells.pivot/pivotfield/filtertop10/
---
## PivotField.FilterTop10 method

Filtra per valori del campo pivot dei dati.

```csharp
public PivotFilter FilterTop10(int valueFieldIndex, PivotFilterType type, bool isTop, int itemCount)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valueFieldIndex | Int32 | L'indice del campo dati nella regione dei dati. |
| type | PivotFilterType | Il tipo di filtraggio dei dati. Può essere solo Count, Sum e Percent. |
| isTop | Booleano | Indica se il filtro è dall'alto o dal basso |
| itemCount | Int32 | Il conteggio degli elementi |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterTop10WithInt32PivotFilterTypeBooleanIntDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            worksheet.Cells["A7"].Value = "Banana";
            worksheet.Cells["A8"].Value = "Apple";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 40;
            worksheet.Cells["B6"].Value = 50;
            worksheet.Cells["B7"].Value = 60;
            worksheet.Cells["B8"].Value = 70;

            // Crea tabella pivot
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B8", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Aggiungi campo dati
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Applica filtro top 10
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableFilterTop10.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


