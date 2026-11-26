---
title: "JsonLayoutOptions.TitleStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLayoutOptions. Obtiene y establece el estilo del título"
type: docs
url: /es/net/aspose.cells.utility/jsonlayoutoptions/titlestyle/
---
## JsonLayoutOptions.TitleStyle property

Obtiene y establece el estilo del título.

```csharp
public Style TitleStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyTitleStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos JSON de ejemplo
            string jsonInput = @"
            {
                ""Name"": ""John"",
                ""Age"": 30,
                ""JoinDate"": ""2023-05-15""
            }";

            // Crear estilo personalizado para los títulos
            CellsFactory factory = new CellsFactory();
            Style titleStyle = factory.CreateStyle();
            titleStyle.HorizontalAlignment = TextAlignmentType.Center;
            titleStyle.Font.Color = System.Drawing.Color.BlueViolet;
            titleStyle.Font.IsBold = true;

            // Configurar opciones de importación de JSON
            JsonLayoutOptions options = new JsonLayoutOptions();
            options.ArrayAsTable = true;
            options.TitleStyle = titleStyle;
            options.ConvertNumericOrDate = true;
            options.DateFormat = "yyyy-MM-dd";

            // Importar datos JSON con estilo de título personalizado
            JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);

            // Ajustar automáticamente las columnas para una mejor visibilidad
            worksheet.AutoFitColumns();

            // Guarda el libro de trabajo
            workbook.Save("JsonWithStyledTitles.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../../aspose.cells/style/)
* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


