---
title: "Cell.SetCharacters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Establece el formato de texto enriquecido de la celda"
type: docs
url: /es/net/aspose.cells/cell/setcharacters/
---
## Cell.SetCharacters method

Establece el formato de texto enriquecido de la celda.

```csharp
public void SetCharacters(FontSetting[] characters)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| caracteres | FontSetting[] | Todos los objetos Characters. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellMethodSetCharactersWithFontSettingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Establecer el valor de la celda para aplicar formato de texto enriquecido
            cell.Value = "Hello World!";

            try
            {
                // Crear configuraciones de fuente para diferentes partes del texto
                FontSetting[] fontSettings = new FontSetting[2];

                // Formatear los primeros 5 caracteres (Hello) como rojo negrita
                fontSettings[0] = cell.Characters(0, 5);
                fontSettings[0].Font.IsBold = true;
                fontSettings[0].Font.Color = Color.Red;

                // Formatear los caracteres restantes ( World!) como azul cursiva
                fontSettings[1] = cell.Characters(5, 7);
                fontSettings[1].Font.IsItalic = true;
                fontSettings[1].Font.Color = Color.Blue;

                // Aplicar la configuración de caracteres formateados usando SetCharacters
                cell.SetCharacters(fontSettings);

                Console.WriteLine("SetCharacters executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCharacters: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


