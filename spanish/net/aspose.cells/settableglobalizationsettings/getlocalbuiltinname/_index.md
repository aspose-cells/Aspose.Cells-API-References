---
title: "SettableGlobalizationSettings.GetLocalBuiltInName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el texto dependiente de la configuración regional para el nombre incorporado según el texto estándar proporcionado"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/getlocalbuiltinname/
---
## SettableGlobalizationSettings.GetLocalBuiltInName method

Obtiene el texto dependiente de la configuración regional para el Nombre incorporado según el texto estándar proporcionado.

```csharp
public override string GetLocalBuiltInName(string standardName)
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

    public class SettableGlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una instancia de SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Llamar al método GetLocalBuiltInName con un nombre incorporado estándar
                string standardName = "SUM";
                string localName = globalizationSettings.GetLocalBuiltInName(standardName);

                // Mostrar el resultado
                Console.WriteLine($"Standard name: {standardName}, Local name: {localName}");

                // Establecer un nombre local personalizado para el nombre incorporado estándar
                globalizationSettings.SetLocalBuiltInName(standardName, "CustomSum", true);

                // Obtener nuevamente el nombre local después de configurarlo
                localName = globalizationSettings.GetLocalBuiltInName(standardName);
                Console.WriteLine($"After setting - Standard name: {standardName}, Local name: {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("MethodGetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


