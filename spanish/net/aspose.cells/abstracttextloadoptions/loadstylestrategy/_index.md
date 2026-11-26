---
title: "AbstractTextLoadOptions.LoadStyleStrategy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AbstractTextLoadOptions. Indica la estrategia para aplicar estilo a los valores analizados al convertir un valor de cadena a número o fecha y hora"
type: docs
url: /es/net/aspose.cells/abstracttextloadoptions/loadstylestrategy/
---
## AbstractTextLoadOptions.LoadStyleStrategy property

Indica la estrategia para aplicar estilo a los valores analizados al convertir una cadena a número o fecha y hora.

```csharp
public TxtLoadStyleStrategy LoadStyleStrategy { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AbstractTextLoadOptionsPropertyLoadStyleStrategyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establezca un estilo personalizado para la demostración
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.Name = "Arial";
            customStyle.Font.Size = 12;
            customStyle.Font.Color = System.Drawing.Color.Blue;
            customStyle.Pattern = BackgroundType.Solid;
            customStyle.ForegroundColor = System.Drawing.Color.LightYellow;

            // Aplicar el estilo a una celda
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(customStyle);

            // Crear datos CSV
            string csvData = "Data1,Data2\nValue1,Value2";
            byte[] byteArray = Encoding.ASCII.GetBytes(csvData);
            MemoryStream stream = new MemoryStream(byteArray);

            // Crear opciones de carga de texto con LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn
            };

            // Importar los datos CSV con las opciones de carga especificadas
            cells.ImportCSV(stream, loadOptions, 0, 0);

            // Guardar el libro de trabajo para demostrar el resultado
            workbook.Save("LoadStyleStrategyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [TxtLoadStyleStrategy](../../txtloadstylestrategy/)
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


