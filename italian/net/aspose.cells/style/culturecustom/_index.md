---
title: "Style.CultureCustom"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Style. Ottiene e imposta la stringa di modello dipendente dalla cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa di modello corrispondente al numero incorporato."
type: docs
url: /it/net/aspose.cells/style/culturecustom/
---
## Style.CultureCustom property

Ottiene e imposta la stringa di modello dipendente dalla cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa di modello corrispondente al numero incorporato.

```csharp
public string CultureCustom { get; set; }
```

### Osservazioni

Per i formati numerici incorporati, sia il contenuto del modello (ad esempio, un formato data incorporato è "m/d/y" per alcune località, ma per altre località diventa "d/m/y") sia il specificatore di formato (ad esempio, alcune località usano un carattere diverso da 'y' per rappresentare la parte dell'anno nella formattazione delle date) sono dipendenti dalla cultura; per i formati personalizzati specificati dall'utente, solo i specificatori di formato vengono modificati in base alla cultura, le altre parti del modello di formattazione non verranno modificate.

### Esempi

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyCultureCustomDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro e imposta la cultura ungherese
            Workbook wb = new Workbook();
            wb.Settings.CultureInfo = new CultureInfo("hu-HU");

            // Ottieni la prima cella e il suo stile
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            Style style = cell.GetStyle();

            // Imposta un formato personalizzato e dimostra la conversione CultureCustom
            string customFormat = "yyyy-MM-dd hh:mm:ss ddd dddd MMM MMMM MMMMM";
            string cultureCustomFormat = "éééé-hh-nn óó:pp:mm nnn nnnn hhh hhhh hhhhh";
            
            style.Custom = customFormat;
            Console.WriteLine("CultureCustom from Custom: " + style.CultureCustom);
            
            style.CultureCustom = cultureCustomFormat;
            Console.WriteLine("Custom from CultureCustom: " + style.Custom);

            // Applica lo stile e dimostra la formattazione sensibile alla cultura
            cell.SetStyle(style);
            cell.PutValue(47512); // January 29, 2030
            Console.WriteLine("Formatted value: " + cell.StringValue);

            // Dimostra la formula con formattazione culturale
            cell.Formula = "=TEXT(47512,\"" + cultureCustomFormat + "\")";
            wb.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.StringValue);
        }
    }
}
```

### Vedi anche

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


