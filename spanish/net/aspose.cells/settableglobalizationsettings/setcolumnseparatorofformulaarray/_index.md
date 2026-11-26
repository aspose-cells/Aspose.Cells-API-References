---
title: "SettableGlobalizationSettings.SetColumnSeparatorOfFormulaArray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el separador para los elementos en los datos de fila de matrices en la fórmula"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/setcolumnseparatorofformulaarray/
---
## SettableGlobalizationSettings.SetColumnSeparatorOfFormulaArray method

Establece el separador para los elementos en los datos de fila de la matriz en la fórmula.

```csharp
public void SetColumnSeparatorOfFormulaArray(char c)
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

    public class SettableGlobalizationSettingsMethodSetColumnSeparatorOfFormulaArrayWithCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
            
            try
            {
                globalizationSettings.SetColumnSeparatorOfFormulaArray('|');
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                worksheet.Cells["A1"].SetArrayFormula("{1|2|3}", 1, 3);
                Console.WriteLine("Column separator for formula arrays set to '|'.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetColumnSeparatorOfFormulaArray: {ex.Message}");
            }

            workbook.Save("SetColumnSeparatorOfFormulaArrayWithCharDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


