---
title: "SettableGlobalizationSettings.ListSeparator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SettableGlobalizationSettings. Obtiene el separador para los parámetros de lista de la función ...etc"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/listseparator/
---
## SettableGlobalizationSettings.ListSeparator property

Obtiene el separador para la lista, los parámetros de la función, ...etc.

```csharp
public override char ListSeparator { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una instancia de SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Mostrar el valor actual de ListSeparator (el predeterminado es coma en la mayoría de configuraciones regionales)
            Console.WriteLine("Current ListSeparator value: " + settings.ListSeparator);
            
            // Establecer un nuevo valor de ListSeparator (p. ej., punto y coma)
            settings.SetListSeparator(';');
            
            // Aplicar la configuración al workbook
            workbook.Settings.GlobalizationSettings = settings;
            
            // Demostrar el efecto de ListSeparator en el análisis de fórmulas
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue("Data");
            
            // Crear una fórmula que utilice el separador de lista
            worksheet.Cells["A3"].Formula = "=CONCATENATE(A1,A2)";
            
            // La fórmula usará el separador de lista personalizado al analizarse
            Console.WriteLine("Formula with custom separator: " + worksheet.Cells["A3"].Formula);
            
            // Guarda el libro de trabajo
            workbook.Save("PropertyListSeparatorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


