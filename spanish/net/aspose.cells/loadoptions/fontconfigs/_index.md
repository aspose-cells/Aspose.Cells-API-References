---
title: "LoadOptions.FontConfigs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Obtiene y establece configuraciones de fuentes individuales. Solo funciona para el Workbook que utiliza este LoadOptions para cargar"
type: docs
url: /es/net/aspose.cells/loadoptions/fontconfigs/
---
## LoadOptions.FontConfigs property

Obtiene y establece configuraciones de fuentes individuales. Solo funciona para el [`Workbook`](../../workbook/) que utiliza este [`LoadOptions`](../) para cargar.

```csharp
public IndividualFontConfigs FontConfigs { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyFontConfigsDemo
    {
        public static void Run()
        {
            // Cree opciones de carga con FontConfigs
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                FontConfigs = new IndividualFontConfigs()
            };

            // Establezca algunas reglas de sustitución de fuentes usando la API correcta
            loadOptions.FontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman" });
            loadOptions.FontConfigs.SetFontSubstitutes("Courier New", new string[] { "Consolas" });

            // Cargar un archivo CSV con las opciones especificadas
            Workbook workbook = new Workbook("sample.csv", loadOptions);

            // Guarda el libro de trabajo en un archivo Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [IndividualFontConfigs](../../individualfontconfigs/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


