---
title: "AbstractGlobalizationSettings.Compare"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractGlobalizationSettings. Compara dos valores de cadena según ciertas reglas de ordenación"
type: docs
url: /es/net/aspose.cells/abstractglobalizationsettings/compare/
---
## AbstractGlobalizationSettings.Compare method

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

    public class AbstractGlobalizationSettingsMethodCompareWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crear configuraciones de globalización personalizadas que sobrescriban el método Compare
            var settings = new CustomGlobalizationSettings();
            
            // Crear un libro de trabajo con configuraciones de globalización personalizadas
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = settings;

            // Preparar cadenas para comparar
            string string1 = "Apple";
            string string2 = "apple";
            bool ignoreCase = true;

            try
            {
                // El método Compare será llamado internamente durante operaciones como la ordenación
                // Demostramos el uso directo aquí
                int comparisonResult = settings.Compare(string1, string2, ignoreCase);
                
                Console.WriteLine($"Comparison result: {comparisonResult}");
                Console.WriteLine($"Strings compared: '{string1}' and '{string2}' (Ignore case: {ignoreCase})");

                // Demostrar el efecto ordenando datos
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Orange");
                worksheet.Cells["A2"].PutValue("apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Apple");

                // Crear un DataSorter y establecer el rango para la ordenación
                DataSorter sorter = workbook.DataSorter;
                sorter.AddKey(0, SortOrder.Ascending);

                sorter.Sort(worksheet.Cells, 0, 0, 3, 0);
                workbook.Save("StringComparisonDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during string comparison: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return String.Compare(v1, v2, ignoreCase);
            }
        }
    }
}
```

### Ver también

* class [AbstractGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


