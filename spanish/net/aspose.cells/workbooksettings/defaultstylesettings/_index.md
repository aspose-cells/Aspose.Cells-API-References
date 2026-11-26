---
title: "WorkbookSettings.DefaultStyleSettings"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "WorkbookSettings property. Obtiene la configuración de los valores predeterminados de las propiedades relacionadas con el estilo para este libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbooksettings/defaultstylesettings/
---
## WorkbookSettings.DefaultStyleSettings property

Obtiene la configuración de los valores predeterminados de las propiedades relacionadas con estilos para este libro.

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Ejemplos

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración de estilo predeterminada
            DefaultStyleSettings styleSettings = workbook.Settings.DefaultStyleSettings;

            // Establecer la preferencia de formato numérico incorporado
            styleSettings.BuiltInPreference = true;

            // Establecer la cultura para el formato de números
            workbook.Settings.CultureInfo = new CultureInfo("en-US");

            // Acceder a las celdas y aplicar formato
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer valores y estilos
            cells["A1"].PutValue(1234.56);
            cells["A1"].GetStyle().Number = 4; // Currency format

            cells["B1"].PutValue(0.456);
            cells["B1"].GetStyle().Number = 2; // Percentage format

            cells["C1"].PutValue(DateTime.Now);
            cells["C1"].GetStyle().Number = 22; // Short date format

            // Guarda el libro de trabajo
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


