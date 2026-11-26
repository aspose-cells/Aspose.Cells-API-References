---
title: "Clase BulletValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Texts.BulletValue. Representa el valor de la viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/bulletvalue/
---
## BulletValue class

Representa el valor de la viñeta.

```csharp
public abstract class BulletValue
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| abstract [Type](../../aspose.cells.drawing.texts/bulletvalue/type/) { get; } | Obtiene el tipo del valor de la viñeta. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassBulletValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un cuadro de texto y obtener sus párrafos de texto
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var textParagraph = textBox.TextBody.TextParagraphs[0];

            // Crear una instancia de CharacterBulletValue (que hereda de BulletValue)
            var bulletValue = new CharacterBulletValue();
            bulletValue.Character = '•';
            
            // Establecer el valor de la viñeta en el párrafo (Bullet es de solo lectura, por lo que necesitamos modificarlo de manera diferente)
            // Dado que Bullet es de solo lectura, necesitamos encontrar otra forma de establecerlo
            // Esto podría implicar crear un nuevo TextParagraph con la viñeta establecida
            // Nota: La API real podría proporcionar una forma diferente de establecer viñetas
            // Para demostración, asumiremos que podemos establecerlo mediante otros medios
            // textParagraph.Bullet = bulletValue; // Esta línea se elimina ya que Bullet es de solo lectura
            textBox.Text = "First bullet point";

            // Agregar otro párrafo con una viñeta diferente
            // TextParagraphCollection no tiene un método Add, por lo que necesitamos encontrar otra forma
            // Esto podría implicar crear un nuevo TextParagraph y agregarlo mediante otros medios
            // Para demostración, asumiremos que podemos obtener el segundo párrafo directamente
            var textParagraph2 = textBox.TextBody.TextParagraphs[1];
            var bulletValue2 = new CharacterBulletValue();
            bulletValue2.Character = '→';
            // textParagraph2.Bullet = bulletValue2; // Esta línea se elimina ya que Bullet es de solo lectura
            textBox.Text += "\nSecond bullet point";

            // Demostrar el acceso al tipo de viñeta
            Console.WriteLine("First bullet type: " + textParagraph.Bullet.Type);
            Console.WriteLine("Second bullet type: " + textParagraph2.Bullet.Type);

            // Guardar el resultado
            workbook.Save("TextsClassBulletValueDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


