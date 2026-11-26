---
title: "Title.Characters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Title. Obtiene el formato de texto enriquecido de este Título"
type: docs
url: /es/net/aspose.cells.charts/title/characters/
---
## Title.Characters method

Obtiene el formato de texto enriquecido de este título.

```csharp
public FontSetting[] Characters()
```

### Valor de retorno

devuelve una matriz de FontSetting

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TitleMethodCharactersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["B3"].PutValue(5);

            // Crear un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Establecer título del gráfico
            chart.Title.Text = "Fruit Sales Report";
            chart.Title.IsVisible = true;

            try
            {
                // Obtenga el formato de texto enriquecido del título
                FontSetting[] titleCharacters = chart.Title.Characters();
                
                // Modifique la fuente del primer carácter
                if (titleCharacters.Length > 0)
                {
                    titleCharacters[0].Font.Color = System.Drawing.Color.Red;
                    titleCharacters[0].Font.IsBold = true;
                    titleCharacters[0].Font.Size = 14;
                }

                Console.WriteLine("Characters method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Characters method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("TitleMethodCharactersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


