---
title: "SettableGlobalizationSettings.GetErrorValueString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el valor de cadena de visualización para el valor de error de las celdas"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/geterrorvaluestring/
---
## SettableGlobalizationSettings.GetErrorValueString method

Obtiene la cadena de visualización del valor de error de la celda

```csharp
public override string GetErrorValueString(string err)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| err | String | valores de error como #VALUE!,#NAME? |

### Valor de retorno

Por defecto devuelve el propio valor de error

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetErrorValueStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            // Crear una celda con valor de error
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("#N/A");
            Style style = workbook.CreateStyle();
            cell.SetStyle(style);
            style.Number = 10; // Set format to Error value

            try
            {
                // Llamar a GetErrorValueString con la cadena de valor de error
                string errorString = settings.GetErrorValueString("#N/A");
                
                // Mostrar el resultado
                Console.WriteLine("Error value string: " + errorString);

                // Mostrar el efecto estableciendo el valor de otra celda a la cadena devuelta
                worksheet.Cells["A2"].PutValue("Error representation: " + errorString);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


