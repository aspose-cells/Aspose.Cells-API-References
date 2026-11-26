---
title: "PivotGlobalizationSettings.GetTextOf4Quaters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene el texto local de 4 trimestres"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/
---
## PivotGlobalizationSettings.GetTextOf4Quaters method

Obtiene el texto local de 4 trimestres.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOf4Quarters() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string[] GetTextOf4Quaters()
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método PivotGlobalizationSettings.GetTextOf4Quarters(). Esta propiedad será eliminada 12 meses después a partir de julio de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetTextOf4QuatersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree una clase de configuración de globalización personalizada que herede de PivotGlobalizationSettings
            var customGlobalizationSettings = new CustomPivotGlobalizationSettings();

            try
            {
                // Llamar al método GetTextOf4Quaters
                string[] quarterNames = customGlobalizationSettings.GetTextOf4Quaters();

                // Mostrar los nombres de los trimestres en la consola
                Console.WriteLine("Names of 4 quarters:");
                foreach (string quarterName in quarterNames)
                {
                    Console.WriteLine(quarterName);
                }

                // Agregar los nombres de los trimestres a la hoja de cálculo
                for (int i = 0; i < quarterNames.Length; i++)
                {
                    worksheet.Cells[i, 0].PutValue(quarterNames[i]);
                }

                Console.WriteLine("Method executed successfully. Quarter names added to worksheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOf4Quaters method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("MethodGetTextOf4QuatersDemo.xlsx");
        }
    }

    // Implementación personalizada de PivotGlobalizationSettings para sobrescribir GetTextOf4Quaters
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetTextOf4Quaters()
        {
            // Devolver nombres de trimestre personalizados
            return new string[] { "First Quarter", "Second Quarter", 
                               "Third Quarter", "Fourth Quarter" };
        }
    }
}
```

### Ver también

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


