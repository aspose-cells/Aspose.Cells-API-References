---
title: "Classe CellsDataTableFactory"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.CellsDataTableFactory. Utility per creare ICellsDataTable da oggetti personalizzati per comodità degli utenti"
type: docs
url: /it/net/aspose.cells/cellsdatatablefactory/
---
## CellsDataTableFactory class

Utility per costruire ICellsDataTable da oggetti personalizzati per la comodità dell'utente.

```csharp
public class CellsDataTableFactory
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance)(double[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_6)(ICollection) | Crea ICellsDataTable dalla collezione fornita. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_3)(int[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_8)(object[]) |  |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_1)(double[], bool) | Crea ICellsDataTable da una sequenza di valori double fornita. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_2)(double[], string[]) | Crea ICellsDataTable da una sequenza di valori double fornita. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_7)(ICollection, bool) | Crea ICellsDataTable dalla collezione fornita. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_4)(int[], bool) | Crea ICellsDataTable da una sequenza di valori interi fornita. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_5)(int[], string[]) | Crea ICellsDataTable da una sequenza di valori interi fornita. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_9)(object[], bool) | Crea ICellsDataTable da una sequenza di oggetti fornita. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_10)(object[], string[]) | Crea ICellsDataTable da una sequenza di oggetti fornita. |
| [GetInstance](../../aspose.cells/cellsdatatablefactory/getinstance/#getinstance_11)(object[][], bool, string[]) | Crea un ICellsDataTable da una sequenza di oggetti fornita. |

### Esempi

```csharp
using Aspose.Cells;
using System;
using System.Collections.Generic;

namespace AsposeCellsExamples
{
    public class CellsDataTableFactoryDemo
    {
        public static void RunDemo()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            List<CustomData> dataList = new List<CustomData>
            {
                new CustomData { Id = 1, Name = "John Doe", Age = 30 },
                new CustomData { Id = 2, Name = "Jane Smith", Age = 25 },
                new CustomData { Id = 3, Name = "Sam Brown", Age = 35 }
            };

            // Ottieni l'istanza di CellsDataTableFactory dalla cartella di lavoro
            CellsDataTableFactory factory = workbook.CellsDataTableFactory;

            // Crea un'istanza di ICellsDataTable dall'elenco di dati personalizzati
            ICellsDataTable dataTable = factory.GetInstance(dataList);

            // Importa la tabella dati nel foglio di lavoro a partire dalla cella A1
            sheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

            // Salva la cartella di lavoro
            workbook.Save("CellsDataTableFactoryDemo.xlsx");
            workbook.Save("CellsDataTableFactoryDemo.pdf");
        }
    }

    // Classe di dati personalizzati
    public class CustomData
    {
        public int Id { get; set; }
        public string Name { get; set; }
        public int Age { get; set; }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


