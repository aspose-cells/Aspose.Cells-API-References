---
title: "XlsSaveOptions.LightCellsDataProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà XlsSaveOptions. Il provider di dati per salvare la cartella di lavoro in modalità leggera"
type: docs
url: /it/net/aspose.cells/xlssaveoptions/lightcellsdataprovider/
---
## XlsSaveOptions.LightCellsDataProvider property

Il provider di dati per salvare la cartella di lavoro in modalità leggera.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Crea le opzioni di salvataggio XLS
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            
            // Imposta il LightCellsDataProvider
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();
            
            // Salva la cartella di lavoro in modalità LightCells
            workbook.Save("output.xls", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        public bool IsGatherString()
        {
            return true;
        }

        public int NextCell()
        {
            return 0; // Only process first cell for demonstration
        }

        public int NextRow()
        {
            return 0; // Only process first row for demonstration
        }

        public void StartCell(Cell cell)
        {
            // Imposta un valore stringa lungo per dimostrare la gestione LightCells
            cell.PutValue(new string('X', 257));
        }

        public void StartRow(Row row)
        {
            // Nessuna gestione speciale delle righe necessaria per questa demo
        }

        public bool StartSheet(int sheetIndex)
        {
            // Nessuna gestione speciale dei fogli necessaria per questa demo
            return false;
        }
    }
}
```

### Vedi anche

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


