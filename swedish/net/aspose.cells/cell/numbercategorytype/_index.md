---
title: "Cell.NumberCategoryType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Representerar kategori-typen för denna cells talformatering"
type: docs
url: /sv/net/aspose.cells/cell/numbercategorytype/
---
## Cell.NumberCategoryType property

Anger kategoritypen för den här cellens talformat.

```csharp
public NumberCategoryType NumberCategoryType { get; }
```

### Anmärkningar

När en cells formateringsmönster kombineras med villkorsformateringsmönster, blir den returnerade typen motsvarande den del som används för cellens aktuella värde. Till exempel, om formateringsmönstret för denna cell är \"#,##0;(#,##0);\"-\";@\", så när cellens värde är numeriskt och inte 0, är den returnerade typen Number; När cellens värde är 0 eller inte är ett numeriskt värde, är den returnerade typen Text.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyNumberCategoryTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ett datumvärde i cell A1
            Cell dateCell = worksheet.Cells["A1"];
            dateCell.PutValue(DateTime.Now);
            
            // Ange datumformat
            Style dateStyle = dateCell.GetStyle();
            dateStyle.Custom = "yyyy-mm-dd";
            dateCell.SetStyle(dateStyle);
            
            // Lägg till ett numeriskt värde i cell A2
            Cell numberCell = worksheet.Cells["A2"];
            numberCell.PutValue(1234.56);
            
            // Lägg till ett textvärde i cell A3
            Cell textCell = worksheet.Cells["A3"];
            textCell.PutValue("Sample Text");
            
            // Visa NumberCategoryType för varje cell
            Console.WriteLine("A1 (Date) NumberCategoryType: " + dateCell.NumberCategoryType);
            Console.WriteLine("A2 (Number) NumberCategoryType: " + numberCell.NumberCategoryType);
            Console.WriteLine("A3 (Text) NumberCategoryType: " + textCell.NumberCategoryType);
            
            // Ändra A2 till valutaformat och kontrollera NumberCategoryType
            Style currencyStyle = numberCell.GetStyle();
            currencyStyle.Custom = "$#,##0.00";
            numberCell.SetStyle(currencyStyle);
            Console.WriteLine("A2 (Currency) NumberCategoryType: " + numberCell.NumberCategoryType);
        }
    }
}
```

### Se även

* enum [NumberCategoryType](../../numbercategorytype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


