---
title: "LightCellsDataProvider.NextRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LightCellsDataProvider. Получает следующую строку для сохранения"
type: docs
url: /ru/net/aspose.cells/lightcellsdataprovider/nextrow/
---
## LightCellsDataProvider.NextRow method

Получает следующую строку для сохранения.

```csharp
public int NextRow()
```

### Возвращаемое значение

индекс следующей строки для сохранения. -1 означает, что достигнут конец данных текущего листа и дальнейшие строки текущего листа сохранять не нужно.

### Примечания

Он будет вызываться в начале сохранения строки и данных её ячеек (до [`StartRow`](../startrow/)).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodNextRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            workbook.Worksheets.Add("Sheet1");

            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            try
            {
                workbook.Save("LightCellsDataProviderMethodNextRowDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with LightCellsDataProvider implementation.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;
        private readonly int totalRows = 3;

        public bool StartSheet(int sheetIndex)
        {
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            currentRow++;
            currentCell = -1;
            return currentRow < totalRows ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            row.Height = 20;
        }

        public int NextCell()
        {
            currentCell++;
            return currentCell < 2 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            return false;
        }
    }
}
```

### См. также

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


