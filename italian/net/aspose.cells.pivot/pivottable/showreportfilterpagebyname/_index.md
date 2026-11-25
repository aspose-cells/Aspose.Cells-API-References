---
title: "PivotTable.ShowReportFilterPageByName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotTable. Mostra tutte le pagine del filtro report secondo il nome dei PivotFields; il PivotField deve essere posizionato nei PageFields"
type: docs
url: /it/net/aspose.cells.pivot/pivottable/showreportfilterpagebyname/
---
## PivotTable.ShowReportFilterPageByName method

Mostra tutte le pagine di filtro del report in base al nome di PivotField, il PivotField deve trovarsi nei PageFields.

```csharp
public void ShowReportFilterPageByName(string fieldName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldName | String | Il nome del PivotField |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByNameWithStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            var cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            
            // Crea tabella pivot
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campi di riga e di dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Aggiungi campo pagina
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Fruit");
            pivotTable.PageFields[0].Name = "FruitFilter";
            
            // Aggiorna la tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Mostra le pagine del filtro report per nome
            pivotTable.ShowReportFilterPageByName("FruitFilter");
            
            // Salva la cartella di lavoro
            workbook.Save("PivotTableShowReportFilterPageByNameDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


