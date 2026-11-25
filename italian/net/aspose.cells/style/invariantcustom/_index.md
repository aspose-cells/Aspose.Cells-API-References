---
title: "Style.InvariantCustom"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene la stringa di modello indipendente dalla cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa di modello corrispondente al numero incorporato."
type: docs
url: /it/net/aspose.cells/style/invariantcustom/
---
## Style.InvariantCustom property

Ottiene la stringa di modello indipendente dalla cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa di modello corrispondente al numero incorporato.

```csharp
public string InvariantCustom { get; }
```

### Osservazioni

Per i formati numerici incorporati, il contenuto del modello restituito è ancora dipendente dalla cultura, ad esempio, per alcune impostazioni regionali restituisce "m/d/y" e per altre restituisce "d/m/y". La differenza rispetto a [`CultureCustom`](../culturecustom/) è (cioè è anche ciò che significa indipendente dalla cultura): i specificatori di formato e i separatori sono mantenuti come standard, ad esempio '/' sarà sempre usato come separatore di data/ora e "y" sarà sempre usato come parte "anno" indipendentemente dal carattere speciale utilizzato per la specifica impostazione regionale.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyInvariantCustomDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Germany;
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();
            
            // Imposta il formato data e il valore
            style.Number = 14; // Date format
            style.Custom = "dd/MM/yyyy"; // Set custom format which affects both CultureCustom and InvariantCustom
            cell.PutValue(new DateTime(2019, 10, 12));
            cell.SetStyle(style);

            // Restituisci i risultati
            Console.WriteLine("Formatted value: " + cell.StringValue);
            Console.WriteLine("CultureCustom: " + style.CultureCustom);
            Console.WriteLine("InvariantCustom: " + style.InvariantCustom);
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


