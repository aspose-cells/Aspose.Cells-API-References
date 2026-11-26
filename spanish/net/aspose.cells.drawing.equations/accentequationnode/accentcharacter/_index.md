---
title: "AccentEquationNode.AccentCharacter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AccentEquationNode. Este atributo especifica el tipo de marca diacrítica combinada adjunta a la base de la función de acento. El carácter de acento predeterminado es U0302. Se recomienda encarecidamente usar el atributo AccentType para establecer el carácter de acento. Utilice esta configuración de propiedad si no puede encontrar el carácter que necesita en un tipo conocido."
type: docs
url: /es/net/aspose.cells.drawing.equations/accentequationnode/accentcharacter/
---
## AccentEquationNode.AccentCharacter property

Este atributo especifica el tipo de marca diacrítica combinante adjunta a la base de la función de acento. El carácter de acento predeterminado es U+0302. Se recomienda encarecidamente usar el atributo AccentType para establecer el carácter de acento. Utilice esta configuración de propiedad si no puede encontrar el carácter que necesita en un tipo conocido.

```csharp
public string AccentCharacter { get; set; }
```

### Observaciones

Debe notarse que esta propiedad solo acepta un carácter, y si se pasan varios caracteres, solo se acepta el primer carácter.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class AccentEquationNodePropertyAccentCharacterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una forma de ecuación a la primera hoja de cálculo
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Obtenga el nodo de ecuación y agregue un nodo de acento
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            
            // Establezca el carácter de acento (circunflejo en este caso)
            accentNode.AccentCharacter = "\u0302";

            // Agregue texto base para el acento
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "x";

            // Guarda el libro de trabajo
            workbook.Save("AccentEquationDemo.xlsx");

            // Verifique el archivo guardado cargándolo nuevamente
            Workbook loadedWorkbook = new Workbook("AccentEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            AccentEquationNode loadedAccentNode = (AccentEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            // Salida del carácter de acento para demostrar la propiedad
            Console.WriteLine("Accent Character: " + loadedAccentNode.AccentCharacter);
        }
    }
}
```

### Ver también

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


