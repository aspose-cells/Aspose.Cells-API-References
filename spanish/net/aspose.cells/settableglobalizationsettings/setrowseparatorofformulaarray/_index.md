---
title: "SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el separador para filas en datos de matriz en la fórmula"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/
---
## SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray method

Establece el separador para las filas en los datos de la matriz en la fórmula.

```csharp
public void SetRowSeparatorOfFormulaArray(char c)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| c | Carácter | el separador especificado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Establecer el separador de filas para matrices de fórmula a '|'
            char rowSeparator = '|';
            settings.SetRowSeparatorOfFormulaArray(rowSeparator);

            // Aplicar la configuración al workbook
            workbook.Settings.GlobalizationSettings = settings;

            // Crear una fórmula de matriz en la hoja de cálculo
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            
            try
            {
                // Calcular la fórmula para aplicar los ajustes
                workbook.CalculateFormula();

                // Mostrar la fórmula con el nuevo separador de filas
                Console.WriteLine("Array formula with custom row separator: " + worksheet.Cells["A1"].Formula);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRowSeparatorOfFormulaArray method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("MethodSetRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


