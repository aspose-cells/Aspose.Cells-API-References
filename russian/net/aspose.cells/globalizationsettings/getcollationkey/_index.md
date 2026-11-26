---
title: "GlobalizationSettings.GetCollationKey"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод GlobalizationSettings. Преобразует строку в сравнимый объект в соответствии с определёнными правилами сортировки"
type: docs
url: /ru/net/aspose.cells/globalizationsettings/getcollationkey/
---
## GlobalizationSettings.GetCollationKey method

Преобразует строку в сравнимый объект в соответствии с определёнными правилами сортировки.

```csharp
public virtual IComparable GetCollationKey(string v, bool ignoreCase)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| v | String | Строковое значение должно сравниваться с другими. |
| ignoreCase | Boolean | нужно ли игнорировать регистр при сравнении значений |

### Возвращаемое значение

Объект может использоваться для сравнения или сортировки строковых значений

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetCollationKeyWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CustomGlobalizationSettings settings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            string inputString = "SampleText";
            bool ignoreCase = true;

            try
            {
                IComparable collationKey = settings.GetCollationKey(inputString, ignoreCase);
                Console.WriteLine($"Collation key for '{inputString}' (ignore case {ignoreCase}): {collationKey}");

                worksheet.Cells["A1"].Value = "Cherry";
                worksheet.Cells["A2"].Value = "apple";
                worksheet.Cells["A3"].Value = "Banana";

                DataSorter sorter = workbook.DataSorter;
                sorter.CaseSensitive = !ignoreCase;
                sorter.Sort(worksheet.Cells, 0, 0, 2, 0);

                Console.WriteLine("\nSorted data:");
                int minDataRow = worksheet.Cells.MinDataRow;
                int maxDataRow = worksheet.Cells.MaxDataRow;
                for (int row = minDataRow; row <= maxDataRow; row++)
                {
                    Cell cell = worksheet.Cells[row, 0];
                    Console.WriteLine(cell.StringValue);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCollationKey: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetCollationKeyDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override IComparable GetCollationKey(string v, bool ignoreCase)
        {
            return ignoreCase ? v.ToLowerInvariant() : v;
        }
    }
}
```

### См. также

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


