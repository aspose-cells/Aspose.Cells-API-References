---
title: "Classe CellsFactory"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.CellsFactory class. Utilità per istanziare classi del modello Cells"
type: docs
url: /it/net/aspose.cells/cellsfactory/
---
## CellsFactory class

Utility per istanziare classi del modello Cells.

```csharp
public class CellsFactory
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [CellsFactory](cellsfactory/)() | Il costruttore predefinito. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CreateStyle](../../aspose.cells/cellsfactory/createstyle/)() | Crea un nuovo stile. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsFactoryDemo
    {
        public static void CellsFactoryExample()
        {
            // Crea una nuova istanza di CellsFactory
            CellsFactory factory = new CellsFactory();

            // Usa la factory per creare un nuovo Style
            Style style = factory.CreateStyle();

            // Personalizza lo stile
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            // Crea una nuova cartella di lavoro e foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Applica lo stile a una cella specifica
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Cell");
            cell.SetStyle(style);

            // Salva la cartella di lavoro in un file
            workbook.Save("CellsFactoryExample.xlsx");
            workbook.Save("CellsFactoryExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


