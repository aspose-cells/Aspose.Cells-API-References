---
title: "Classe SmartTagSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Markup.SmartTagSetting. Rappresenta tutti gli oggetti SmartTagCollection nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells.markup/smarttagsetting/
---
## SmartTagSetting class

Rappresenta tutti gli oggetti [`SmartTagCollection`](../smarttagcollection/) nel foglio di lavoro.

```csharp
public class SmartTagSetting : CollectionBase
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Item](../../aspose.cells.markup/smarttagsetting/item/) { get; } | Ottiene un oggetto [`SmartTagCollection`](../smarttagcollection/) per indice. (3 indicizzatori) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add_1)(string) | Aggiungi smart tag a una cella. |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add)(int, int) | Aggiunge un oggetto [`SmartTagCollection`](../smarttagcollection/) a una cella. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingDemo
    {
        public static void SmartTagSettingExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi uno smart tag a una cella specifica
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Adding smart tag to cell A1

            // Accedi alla SmartTagCollection per la cella
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];

            // Aggiungi un tag intelligente alla collezione
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            // Imposta la capacità dell'impostazione del tag intelligente
            smartTagSetting.Capacity = 10;

            // Stampa il conteggio dei tag intelligenti
            Console.WriteLine("Total Smart Tags: " + smartTagSetting.Count);

            // Salva la cartella di lavoro
            workbook.Save("SmartTagSettingExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


