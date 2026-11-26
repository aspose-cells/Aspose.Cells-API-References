---
title: "GlobalizationSettings.GetLocalBuiltInName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el texto dependiente de la configuración regional para builtin Name según el texto estándar proporcionado"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getlocalbuiltinname/
---
## GlobalizationSettings.GetLocalBuiltInName method

Obtiene el texto dependiente de la configuración regional para el Nombre incorporado según el texto estándar proporcionado.

```csharp
public virtual string GetLocalBuiltInName(string standardName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| standardName | String | Texto estándar (configuración regional en-US) del Nombre incorporado. |

### Valor de retorno

Texto dependiente de la configuración regional. La configuración regional fue especificada por el Libro de trabajo para el cual se usa esta configuración.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                string standardName = "Total";
                string localizedName = ((CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings).GetLocalBuiltInName(standardName);

                Console.WriteLine($"Standard Name: {standardName}");
                Console.WriteLine($"Localized Name: {localizedName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            workbook.Save("LocalizedBuiltInNameDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetLocalBuiltInName(string standardName)
        {
            switch (standardName)
            {
                case "Total":
                    return "LocalizedTotal";
                case "Average":
                    return "LocalizedAverage";
                default:
                    return base.GetLocalBuiltInName(standardName);
            }
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


