---
title: "SettableGlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SettableGlobalizationSettings. Obtiene el separador para filas en datos de matriz en la fórmula"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/
---
## SettableGlobalizationSettings.RowSeparatorOfFormulaArray property

Obtiene el separador para las filas en los datos de matriz en la fórmula.

```csharp
public override char RowSeparatorOfFormulaArray { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una instancia de SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // Mostrar el separador de fila predeterminado para matrices de fórmulas
            Console.WriteLine("Default RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // Establecer un nuevo separador de fila para matrices de fórmulas
            settings.SetRowSeparatorOfFormulaArray(';');

            // Aplicar la configuración al workbook
            workbook.Settings.GlobalizationSettings = settings;

            // Crear una fórmula de matriz en la hoja de cálculo
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            worksheet.Cells["A2"].SetArrayFormula("=SUM(A1:C2)", 1, 1);

            // Calcular fórmulas
            workbook.CalculateFormula();

            // Guarda el libro de trabajo
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


