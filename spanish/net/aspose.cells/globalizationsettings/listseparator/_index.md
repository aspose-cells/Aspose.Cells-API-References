---
title: "GlobalizationSettings.ListSeparator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GlobalizationSettings. Obtiene el separador para los parámetros de lista de la función ...etc"
type: docs
url: /es/net/aspose.cells/globalizationsettings/listseparator/
---
## GlobalizationSettings.ListSeparator property

Obtiene el separador para la lista, los parámetros de la función, ...etc.

```csharp
public virtual char ListSeparator { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con configuraciones de globalización personalizadas
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            Worksheet worksheet = workbook.Worksheets[0];
            
            // Muestre el valor actual de ListSeparator de nuestra configuración personalizada
            Console.WriteLine("Current ListSeparator value: " + workbook.Settings.GlobalizationSettings.ListSeparator);

            // Cree una fórmula usando el separador de lista personalizado
            worksheet.Cells["A1"].Formula = "=CONCATENATE(\"Hello\"; \" World\")";
            worksheet.Cells["A2"].Formula = "=SUM(1;2;3)";

            // Calcule fórmulas con el separador personalizado
            workbook.CalculateFormula();

            // Mostrar resultados del cálculo
            Console.WriteLine("Concatenation result: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Sum result: " + worksheet.Cells["A2"].Value);

            // Guarde con fórmulas usando el separador de lista personalizado
            workbook.Save("ListSeparatorDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ListSeparator => ';';
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


