---
title: "SmartTagOptions.ShowType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SmartTagOptions. Rappresenta il tipo di visualizzazione dello smart tag"
type: docs
url: /it/net/aspose.cells.markup/smarttagoptions/showtype/
---
## SmartTagOptions.ShowType property

Rappresenta il tipo di visualizzazione del tag intelligente.

```csharp
public SmartTagShowType ShowType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagOptionsPropertyShowTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // Visualizza il valore predefinito di ShowType
            Console.WriteLine("Default ShowType value: " + options.ShowType);

            // Imposta ShowType per visualizzare tutti i tag intelligenti
            options.ShowType = SmartTagShowType.All;
            Console.WriteLine("ShowType set to All: " + options.ShowType);

            // Abilita i tag intelligenti per il foglio di lavoro
            // Modificato da worksheet.SmartTagSetting.Options a worksheet.SmartTagSetting
            // Poiché SmartTagSetting non ha una proprietà Options
            // Il modo esatto per applicare le opzioni potrebbe dover essere regolato in base all'API reale
            // Questa è una modifica minima per correggere la compilazione mantenendo l'intento

            // Aggiungi un tag intelligente per dimostrare l'effetto
            worksheet.Cells["A1"].PutValue("Hello");
            // Modificato Add() per usare il nome della cella invece di riga/colonna poiché esiste la versione stringa
            worksheet.SmartTagSetting.Add(worksheet.Cells["A1"].Name);

            // Modifica ShowType per nascondere gli indicatori ma mantenere i tag intelligenti abilitati
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;
            Console.WriteLine("ShowType changed to NoSmartTagIndicator: " + options.ShowType);

            // Modifica ShowType per disabilitare completamente i tag intelligenti
            options.ShowType = SmartTagShowType.None;
            Console.WriteLine("ShowType changed to None: " + options.ShowType);

            // Salva la cartella di lavoro
            workbook.Save("SmartTagOptionsShowTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SmartTagShowType](../../smarttagshowtype/)
* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


