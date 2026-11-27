---
title: "JsonSaveOptions.SheetIndexes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonSaveOptions-egenskap. Representerar indexen för exporterade blad"
type: docs
url: /sv/net/aspose.cells/jsonsaveoptions/sheetindexes/
---
## JsonSaveOptions.SheetIndexes property

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

    public class JsonSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med flera blad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Fyll i lite data i varje blad
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from Sheet {i + 1}");
            }

            // Skapa en JsonSaveOptions-instans
            JsonSaveOptions options = new JsonSaveOptions();

            // Visa aktuella SheetIndexes (null som standard – exporterar alla blad)
            Console.WriteLine("Current SheetIndexes: " + (options.SheetIndexes == null ? "Exporting all sheets" : string.Join(",", options.SheetIndexes)));

            // Ställ in att exportera endast första och tredje bladet (index 0 och 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Spara till JSON med valda blad
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo.json", options);

            // Verifiera genom att läsa in JSON‑filen
            string jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo.json");
            Console.WriteLine("JSON Content:");
            Console.WriteLine(jsonContent);

            // Ändra för att exportera endast det andra bladet (index 1)
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json", options);

            // Verifiera export av ett enda blad
            jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json");
            Console.WriteLine("Single Sheet JSON Content:");
            Console.WriteLine(jsonContent);
        }
    }
}
```

### Se även

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


