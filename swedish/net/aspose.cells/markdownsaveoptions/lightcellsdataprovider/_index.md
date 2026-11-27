---
title: "MarkdownSaveOptions.LightCellsDataProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions‑egenskap. Dataleverantören som tillhandahåller celldata för att spara arbetsboken i lätt läge"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/lightcellsdataprovider/
---
## MarkdownSaveOptions.LightCellsDataProvider property

Dataleverantören som tillhandahåller celldata för att spara arbetsboken i lättläge.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections.Generic;

    public class MarkdownSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite exempeldata
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Item " + (i + 1);
                worksheet.Cells[i, 1].Value = i + 1;
            }

            // Skapa anpassad LightCellsDataProvider
            var dataProvider = new CustomLightCellsDataProvider();

            // Skapa MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            
            // Visa aktuellt värde (bör vara null initialt)
            Console.WriteLine("Current LightCellsDataProvider value: " + (saveOptions.LightCellsDataProvider == null ? "null" : "set"));

            // Ange den anpassade dataleverantören
            saveOptions.LightCellsDataProvider = dataProvider;

            // Spara med den anpassade dataleverantören
            workbook.Save("LightCellsDataProviderDemo.md", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private List<string> items = new List<string> { "Apple", "Banana", "Cherry", "Date", "Elderberry" };
        private List<double> values = new List<double> { 1.99, 0.99, 2.99, 3.49, 4.99 };
        private int currentRow = -1;

        public bool StartSheet(int sheetIndex)
        {
            // Bearbeta endast det första bladet
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            currentRow++;
            return currentRow < items.Count ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // Ange radhöjd om det behövs
            row.Height = 15;
        }

        public int NextCell()
        {
            if (currentRow == -1)
            {
                // Rubrikrad
                return currentRow < 2 ? currentRow + 1 : -1;
            }
            else
            {
                return currentRow < 2 ? currentRow + 1 : -1;
            }
        }

        public void StartCell(Cell cell)
        {
            if (currentRow == -1)
            {
                // Sidhuvud
                if (cell.Column == 0)
                    cell.Value = "Product";
                else if (cell.Column == 1)
                    cell.Value = "Price";
            }
            else
            {
                // Data
                if (cell.Column == 0)
                    cell.Value = items[currentRow];
                else if (cell.Column == 1)
                    cell.Value = values[currentRow];
            }
        }

        public bool IsGatherString()
        {
            return false;
        }
    }
}
```

### Se även

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


