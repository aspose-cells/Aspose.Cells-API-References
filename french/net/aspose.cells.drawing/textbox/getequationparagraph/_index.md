---
title: "TextBox.GetEquationParagraph"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode TextBox. Obtient le paragraphe mathématique spécifié à partir de la propriété TextBody de l’objet TextBox. Remarque 1 : renvoie NULL lorsque l’index est hors limites ou introuvable. Remarque 2 : renvoie également NULL si la position d’index spécifiée n’est pas un paragraphe mathématique"
type: docs
url: /fr/net/aspose.cells.drawing/textbox/getequationparagraph/
---
## GetEquationParagraph(int) {#getequationparagraph_1}

Obtient le paragraphe mathématique spécifié de la propriété TextBody de l'objet TextBox. Remarque : (1) Renvoie NULL lorsque l'index est hors limites ou introuvable. (2) Renvoie également NULL si la position d'index spécifiée n'est pas un paragraphe mathématique.

```csharp
public EquationNode GetEquationParagraph(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'index de position du paragraphe mathématique, à partir de 0. |

### Valeur de retour

Renvoie le paragraphe mathématique spécifié par l'index.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class TextBoxMethodGetEquationParagraphWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte à la feuille de calcul
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Ajoutez du contenu d'équation à la zone de texte
            textBox.Text = "\\sqrt{x^2 + y^2}";

            try
            {
                // Appelez GetEquationParagraph avec le paramètre d'index (Int32)
                EquationNode equationNode = textBox.GetEquationParagraph(0);

                if (equationNode != null)
                {
                    Console.WriteLine("Equation paragraph retrieved successfully.");
                    Console.WriteLine($"Equation type: {equationNode.EquationType}");
                    Console.WriteLine($"LaTeX representation: {equationNode.ToLaTeX()}");
                }
                else
                {
                    Console.WriteLine("No equation paragraph found at the specified index.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEquationParagraph method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("TextBoxMethodGetEquationParagraphWithInt32Demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## GetEquationParagraph() {#getequationparagraph}

Obtient le premier paragraphe mathématique de la propriété TextBody de l'objet TextBox.

```csharp
public EquationNode GetEquationParagraph()
```

### Valeur de retour

S'il existe un paragraphe mathématique, renvoie le premier, sinon renvoie null.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class TextBoxMethodGetEquationParagraphDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int textBoxIndex = worksheet.TextBoxes.Add(5, 5, 200, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "$$\\sqrt{x^2+y^2}$$";
            
            EquationNode equationNode = textBox.GetEquationParagraph();
            
            if (equationNode != null)
            {
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                Console.WriteLine("Equation MathML: " + equationNode.ToMathML());
            }
            else
            {
                Console.WriteLine("No equation paragraph found");
            }
        }
    }
}
```

### Voir aussi

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


