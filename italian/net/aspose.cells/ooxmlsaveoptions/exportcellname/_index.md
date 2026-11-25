---
title: "OoxmlSaveOptions.ExportCellName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OoxmlSaveOptions. Indica se esportare il nome della cella in un file Excel2007 .xlsx .xlsm .xltx .xltm. Se il file di output può essere accessibile da SQL Server DTS, questo valore deve essere true. Impostare il valore a false aumenterà notevolmente le prestazioni e ridurrà la dimensione del file quando si creano file di grandi dimensioni. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/ooxmlsaveoptions/exportcellname/
---
## OoxmlSaveOptions.ExportCellName property

Indica se esportare il nome della cella in un file Excel2007 .xlsx (.xlsm, .xltx, .xltm). Se il file di output può essere accessibile da SQL Server DTS, questo valore deve essere true. Impostare il valore a false aumenterà notevolmente le prestazioni e ridurrà le dimensioni del file quando si crea un file di grandi dimensioni. Il valore predefinito è true.

```csharp
public bool ExportCellName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyExportCellNameDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Inserisci alcuni dati nelle celle
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            
            // Crea le opzioni di salvataggio XLSX con ExportCellName abilitato
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.ExportCellName = true;
            
            // Salva la cartella di lavoro con i nomi delle celle esportati
            workbook.Save("output_with_cellnames.xlsx", saveOptions);
            
            // Crea un'altra opzione di salvataggio con ExportCellName disabilitato (predefinito)
            OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
            
            // Salva la cartella di lavoro senza esportare i nomi delle celle
            workbook.Save("output_without_cellnames.xlsx", saveOptions2);
        }
    }
}
```

### Vedi anche

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


