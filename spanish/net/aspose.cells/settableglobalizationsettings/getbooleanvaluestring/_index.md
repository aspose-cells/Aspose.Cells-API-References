---
title: "SettableGlobalizationSettings.GetBooleanValueString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene la cadena de visualización para el valor booleano de las celdas"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/getbooleanvaluestring/
---
## SettableGlobalizationSettings.GetBooleanValueString method

Obtiene la cadena de visualización del valor booleano de la celda

```csharp
public override string GetBooleanValueString(bool bv)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| bv | Booleano | valor booleano |

### Valor de retorno

Por defecto devuelve "TRUE" para el valor verdadero y "FALSE" para el valor falso.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Establecer cadenas de valores booleanos personalizadas
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // Aplicar la configuración al workbook
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Llame a GetBooleanValueString con true
                string trueValue = settings.GetBooleanValueString(true);
                Console.WriteLine("Custom true value: " + trueValue);

                // Llame a GetBooleanValueString con false
                string falseValue = settings.GetBooleanValueString(false);
                Console.WriteLine("Custom false value: " + falseValue);

                // Demuestre el efecto en la hoja de cálculo
                worksheet.Cells["A1"].PutValue(true);
                worksheet.Cells["A2"].PutValue(false);

                Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2 value: " + worksheet.Cells["A2"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBooleanValueString method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("SettableGlobalizationSettingsMethodGetBooleanValueStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


