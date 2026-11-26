---
title: "Clase AbstractGlobalizationSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.AbstractGlobalizationSettings. Representa la configuración de globalización"
type: docs
url: /es/net/aspose.cells/abstractglobalizationsettings/
---
## AbstractGlobalizationSettings class

Representa la configuración de globalización.

```csharp
public abstract class AbstractGlobalizationSettings
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare/)(string, string, bool) | Compara dos valores de cadena según ciertas reglas de ordenación. |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey/)(string, bool) | Transforma la cadena en un objeto comparable según ciertas reglas de ordenación. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAbstractGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // Crear una implementación personalizada de AbstractGlobalizationSettings
            var customSettings = new CustomGlobalizationSettings();

            try
            {
                // Demostrar el método Compare
                string str1 = "Hello";
                string str2 = "hello";
                bool ignoreCase = true;

                int comparisonResult = customSettings.Compare(str1, str2, ignoreCase);
                Console.WriteLine($"Comparison result ({str1} vs {str2}, ignoreCase={ignoreCase}): {comparisonResult}");

                // Demostrar el método GetCollationKey
                string testString = "Sample";
                IComparable collationKey = customSettings.GetCollationKey(testString, ignoreCase);
                Console.WriteLine($"Collation key for '{testString}' (ignoreCase={ignoreCase}): {collationKey}");

                // Aplicar la configuración a un libro de trabajo
                Workbook workbook = new Workbook();
                workbook.Settings.GlobalizationSettings = customSettings;

                // Agregar algunos datos para demostrar la configuración en acción
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Apple");
                worksheet.Cells["A2"].PutValue("banana");
                worksheet.Cells["A3"].PutValue("Cherry");

                // Guarda el libro de trabajo
                workbook.Save("GlobalizationSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved with custom globalization settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override int Compare(string v1, string v2, bool ignoreCase)
            {
                return string.Compare(v1, v2, ignoreCase ? StringComparison.OrdinalIgnoreCase : StringComparison.Ordinal);
            }

            public override IComparable GetCollationKey(string v, bool ignoreCase)
            {
                return ignoreCase ? v.ToLowerInvariant() : v;
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


