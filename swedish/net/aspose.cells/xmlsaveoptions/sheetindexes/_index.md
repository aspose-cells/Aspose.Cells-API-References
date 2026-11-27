---
title: "XmlSaveOptions.SheetIndexes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XmlSaveOptions egenskap. Representerar indexen för exporterade blad"
type: docs
url: /sv/net/aspose.cells/xmlsaveoptions/sheetindexes/
---
## XmlSaveOptions.SheetIndexes property

Representerar indexen för exporterade blad.

```csharp
public int[] SheetIndexes { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med flera blad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Fyll i lite data i alla blad
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue("Data in " + sheet.Name);
            }

            // Skapa XmlSaveOptions‑instans
            XmlSaveOptions options = new XmlSaveOptions();

            // Exportera initialt alla blad (SheetIndexes är null)
            Console.WriteLine("Initial SheetIndexes value: " + (options.SheetIndexes == null ? "null (all sheets)" : string.Join(",", options.SheetIndexes)));

            // Ställ in att exportera endast första och tredje bladet (index 0 och 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Spara endast med valda blad
            workbook.Save("XmlExportSelectedSheets.xml", options);

            // Ändra för att exportera endast det andra bladet (index 1)
            options.SheetIndexes = new int[] { 1 };

            // Spara med olika bladval
            workbook.Save("XmlExportSingleSheet.xml", options);

            // Ställ SheetIndexes till null för att exportera alla blad
            options.SheetIndexes = null;
            workbook.Save("XmlExportAllSheets.xml", options);
        }
    }
}
```

### Se även

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


