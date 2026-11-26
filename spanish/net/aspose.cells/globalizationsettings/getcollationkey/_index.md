---
title: "GlobalizationSettings.GetCollationKey"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Transforma la cadena en un objeto comparable según ciertas reglas de ordenamiento"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getcollationkey/
---
## GlobalizationSettings.GetCollationKey method

Transforma la cadena en un objeto comparable según ciertas reglas de ordenación.

```csharp
public virtual IComparable GetCollationKey(string v, bool ignoreCase)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| v | String | El valor de cadena necesita compararse con otros. |
| ignoreCase | Booleano | si se ignora mayúsculas y minúsculas al comparar valores |

### Valor de retorno

El objeto puede usarse para comparar o ordenar valores de cadena

### Ejemplos

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

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


