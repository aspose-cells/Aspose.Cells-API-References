---
title: "DrawObject.CurrentPage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DrawObject. Indique l'index de page de DrawObject. L'index de page commence à zéro. Une feuille contient plusieurs pages lors du rendu"
type: docs
url: /fr/net/aspose.cells.rendering/drawobject/currentpage/
---
## DrawObject.CurrentPage property

Indique l’indice de page de DrawObject. L’indice de page commence à zéro. Une feuille contient plusieurs pages lors du rendu.

```csharp
public int CurrentPage { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class DrawObjectPropertyCurrentPageDemo
    {
        // Gestionnaire personnalisé pour lire et afficher la propriété CurrentPage
        private class CurrentPageHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                // Affichez la valeur de la propriété CurrentPage
                Console.WriteLine($"CurrentPage: {drawObject.CurrentPage}");
                Console.WriteLine($"TotalPages: {drawObject.TotalPages}");
                Console.WriteLine($"SheetIndex: {drawObject.SheetIndex}");
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine();
            }
        }

        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur et accéder à la première feuille de calcul
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajoutez quelques données d'exemple pour rendre le rendu significatif
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["A2"].PutValue("More Data");
                worksheet.Cells["A3"].Formula = "=A1 & \" \" & A2";

                // Ajoutez une forme pour générer des shape-type draw objects
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 5, 0, 5, 0, 120, 60);
                shape.Text = "Sample Shape";

                // Configurez les options de rendu avec notre gestionnaire de dessin personnalisé
                ImageOrPrintOptions renderOptions = new ImageOrPrintOptions
                {
                    ImageType = ImageType.Png,
                    OnePagePerSheet = true,
                    DrawObjectEventHandler = new CurrentPageHandler()
                };

                // Rendre la feuille de calcul pour déclencher les événements DrawObject
                SheetRender sheetRender = new SheetRender(worksheet, renderOptions);
                sheetRender.ToImage(0, "CurrentPageDemo.png");

                // Enregistrez le classeur
                workbook.Save("CurrentPageDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


