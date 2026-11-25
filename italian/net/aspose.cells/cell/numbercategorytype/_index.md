---
title: "Cell.NumberCategoryType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Rappresenta il tipo di categoria della formattazione numerica di questa cella"
type: docs
url: /it/net/aspose.cells/cell/numbercategorytype/
---
## Cell.NumberCategoryType property

Rappresenta il tipo di categoria della formattazione numerica di questa cella.

```csharp
public NumberCategoryType NumberCategoryType { get; }
```

### Osservazioni

Quando il modello di formattazione della cella è combinato con modelli di formattazione condizionale, il tipo restituito corrisponde alla parte utilizzata per il valore corrente di questa cella. Ad esempio, se il modello di formattazione per questa cella è "#,##0;(#,##0);"-";@", allora quando il valore della cella è numerico e diverso da 0, il tipo restituito è Number; quando il valore della cella è 0 o non è un valore numerico, il tipo restituito è Text.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyNumberCategoryTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un valore data alla cella A1
            Cell dateCell = worksheet.Cells["A1"];
            dateCell.PutValue(DateTime.Now);
            
            // Imposta il formato data
            Style dateStyle = dateCell.GetStyle();
            dateStyle.Custom = "yyyy-mm-dd";
            dateCell.SetStyle(dateStyle);
            
            // Aggiungi un valore numerico alla cella A2
            Cell numberCell = worksheet.Cells["A2"];
            numberCell.PutValue(1234.56);
            
            // Aggiungi un valore di testo alla cella A3
            Cell textCell = worksheet.Cells["A3"];
            textCell.PutValue("Sample Text");
            
            // Visualizza NumberCategoryType per ogni cella
            Console.WriteLine("A1 (Date) NumberCategoryType: " + dateCell.NumberCategoryType);
            Console.WriteLine("A2 (Number) NumberCategoryType: " + numberCell.NumberCategoryType);
            Console.WriteLine("A3 (Text) NumberCategoryType: " + textCell.NumberCategoryType);
            
            // Modifica A2 in formato valuta e verifica NumberCategoryType
            Style currencyStyle = numberCell.GetStyle();
            currencyStyle.Custom = "$#,##0.00";
            numberCell.SetStyle(currencyStyle);
            Console.WriteLine("A2 (Currency) NumberCategoryType: " + numberCell.NumberCategoryType);
        }
    }
}
```

### Vedi anche

* enum [NumberCategoryType](../../numbercategorytype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


