---
title: "Cell.GetCharacters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto de la celda"
type: docs
url: /es/net/aspose.cells/cell/getcharacters/
---
## GetCharacters() {#getcharacters}

Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto de la celda.

```csharp
public FontSetting[] GetCharacters()
```

### Valor de retorno

Todos los objetos Characters

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer texto con formato HTML en la celda A1 con diferentes partes de formato
            worksheet.Cells["A1"].HtmlString = "Normal text<div style=\"color: red;\">Red text</div>";

            // Obtener la información de formato de caracteres de la celda A1
            FontSetting[] fontSettings = worksheet.Cells["A1"].GetCharacters();

            // Mostrar la información de formato
            Console.WriteLine("Character formatting in cell A1:");
            for (int i = 0; i < fontSettings.Length; i++)
            {
                Console.WriteLine($"Part {i + 1}:");
                Console.WriteLine($"Start index: {fontSettings[i].StartIndex}");
                Console.WriteLine($"Length: {fontSettings[i].Length}");
                Console.WriteLine($"Font color: {fontSettings[i].Font.Color}");
                Console.WriteLine();
            }
        }
    }
}
```

### Ver también

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCharacters(bool) {#getcharacters_1}

Devuelve todos los objetos Characters que representan un rango de caracteres dentro del texto de la celda.

```csharp
public FontSetting[] GetCharacters(bool flag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| bandera | Booleano | Indica si se aplica estilo de tabla a la celda cuando la celda está en la tabla. |

### Valor de retorno

Todos los objetos Characters

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetCharactersWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar texto a la celda C8 con formato
            Cell cell = worksheet.Cells["C8"];
            cell.PutValue("Formatted Text");
            
            // Formatear partes del texto
            FontSetting fs1 = cell.Characters(0, 8);
            fs1.Font.Color = System.Drawing.Color.White;
            
            FontSetting fs2 = cell.Characters(9, 4);
            fs2.Font.Color = System.Drawing.Color.Blue;
            
            // Obtener todas las configuraciones de fuente con formato
            FontSetting[] fontSettings = cell.GetCharacters(true);
            
            // Mostrar colores de fuente
            Console.WriteLine("Font colors in cell C8:");
            foreach (FontSetting fs in fontSettings)
            {
                Console.WriteLine(fs.Font.Color);
            }
        }
    }
}
```

### Ver también

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


