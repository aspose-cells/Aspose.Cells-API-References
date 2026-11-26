---
title: "GlobalizationSettings.Compare"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Compara dos valores de cadena según ciertas reglas de ordenamiento"
type: docs
url: /es/net/aspose.cells/globalizationsettings/compare/
---
## GlobalizationSettings.Compare method

Compara dos valores de cadena según ciertas reglas de ordenación.

```csharp
public virtual int Compare(string v1, string v2, bool ignoreCase)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| v1 | String | la primera cadena |
| v2 | String | la segunda cadena |
| ignoreCase | Booleano | si se ignora mayúsculas y minúsculas al comparar valores |

### Valor de retorno

Entero que indica la relación léxica entre los dos comparandos

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo con configuraciones de globalización personalizadas
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomComparisonSettings();

            try
            {
                // Demuestre el uso directo del método Compare
                GlobalizationSettings settings = workbook.Settings.GlobalizationSettings;
                int result1 = settings.Compare("Apple", "apple", true);
                int result2 = settings.Compare("Apple", "apple", false);
                
                Console.WriteLine($"Case-insensitive comparison result: {result1}");
                Console.WriteLine($"Case-sensitive comparison result: {result2}");

                // Demuestre el efecto en las operaciones de la hoja de cálculo
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Banana");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Ordenar datos usando comparación personalizada
                DataSorter sorter = workbook.DataSorter;
                sorter.Order1 = SortOrder.Ascending;
                sorter.Key1 = 0;
                sorter.Sort(worksheet.Cells, 0, 0, 2, 0); // Corrected range to rows 0-2

                Console.WriteLine("Sorted data with custom comparison rules:");
                for (int row = 0; row < 3; row++)
                {
                    Cell cell = worksheet.Cells[row, 0];
                    Console.WriteLine(cell.StringValue);
                }

                workbook.Save("GlobalizationCompareDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomComparisonSettings : GlobalizationSettings
    {
        public override int Compare(string v1, string v2, bool ignoreCase)
        {
            // Implementar lógica de comparación personalizada
            var comparison = ignoreCase ? 
                StringComparison.OrdinalIgnoreCase : 
                StringComparison.Ordinal;
            
            return string.Compare(v1?.Trim() ?? "", v2?.Trim() ?? "", comparison);
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


