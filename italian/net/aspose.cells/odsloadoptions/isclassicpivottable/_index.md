---
title: "OdsLoadOptions.IsClassicPivotTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsLoadOptions. Indica se la tabella pivot è classica"
type: docs
url: /it/net/aspose.cells/odsloadoptions/isclassicpivottable/
---
## OdsLoadOptions.IsClassicPivotTable property

Indica se la tabella pivot è classica.

```csharp
public bool IsClassicPivotTable { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsLoadOptionsPropertyIsClassicPivotTableDemo
    {
        public static void Run()
        {
            // Crea un file ODS di esempio con tabella pivot
            CreateSampleOdsWithPivotTable();

            // Carica con IsClassicPivotTable impostato su true
            OdsLoadOptions loadOptionsTrue = new OdsLoadOptions();
            loadOptionsTrue.IsClassicPivotTable = true;
            
            Workbook workbookTrue = new Workbook("SamplePivot.ods", loadOptionsTrue);
            Console.WriteLine("Loaded with IsClassicPivotTable = true");
            Console.WriteLine("PivotTable fields count: " + workbookTrue.Worksheets[0].PivotTables[0].BaseFields.Count);

            // Carica con IsClassicPivotTable impostato su false
            OdsLoadOptions loadOptionsFalse = new OdsLoadOptions();
            loadOptionsFalse.IsClassicPivotTable = false;
            
            Workbook workbookFalse = new Workbook("SamplePivot.ods", loadOptionsFalse);
            Console.WriteLine("\nLoaded with IsClassicPivotTable = false");
            Console.WriteLine("PivotTable fields count: " + workbookFalse.Worksheets[0].PivotTables[0].BaseFields.Count);
        }

        private static void CreateSampleOdsWithPivotTable()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Popola dati di esempio
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Electronics";
            cells["A3"].Value = "Clothing";
            cells["A4"].Value = "Books";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1500;
            cells["B3"].Value = 800;
            cells["B4"].Value = 200;

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesReport");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi campo riga (Categoria)
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Aggiungi campo dati (Vendite) e imposta il nome visualizzato
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.DataFields[dataFieldIndex].DisplayName = "Total Sales";

            // Salva come ODS
            workbook.Save("SamplePivot.ods", SaveFormat.Ods);
        }
    }
}
```

### Vedi anche

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


