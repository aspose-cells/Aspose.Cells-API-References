---
title: "PivotFilter.MeasureCubeFieldIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotFilter. Specifica l'indice del campo cubo di misura. Questa proprietà è usata solo dai filtri nei pivot OLAP e specifica su quale misura deve essere applicato un filtro di valore"
type: docs
url: /it/net/aspose.cells.pivot/pivotfilter/measurecubefieldindex/
---
## PivotFilter.MeasureCubeFieldIndex property

Specifica l'indice del campo cubo di misura. Questa proprietà è usata solo dai filtri nelle pivot OLAP e specifica su quale misura deve essere applicato un filtro di valore.

```csharp
public int MeasureCubeFieldIndex { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyMeasureCubeFieldIndexDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e riempilo con dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // Aggiungi una tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Aggiungi campi di riga e di dati
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Aggiorna i dati della tabella pivot
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Aggiungi un filtro alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField field = pivotTable.BaseFields[0];
            
            // Crea e aggiungi il filtro tramite PivotTable invece di PivotField
            int filterIndex = pivotTable.PivotFilters.Add(field.Position, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            
            // Visualizza MeasureCubeFieldIndex
            Console.WriteLine("MeasureCubeFieldIndex: " + filter.MeasureCubeFieldIndex);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotFilterMeasureCubeFieldIndexDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


