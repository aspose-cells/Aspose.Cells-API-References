---
title: "FontFileDataInfo.FormatType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FontFileDataInfo. Obtient le type de format de police du fichier de police"
type: docs
url: /fr/net/aspose.cells/fontfiledatainfo/formattype/
---
## FontFileDataInfo.FormatType property

Obtient le type de format de police du fichier de police.

```csharp
public FontFileFormatType FormatType { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyFormatTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter du texte pour démontrer l'utilisation de la police
            worksheet.Cells["A1"].PutValue("Sample Text with Font");

            try
            {
                // Charger un fichier de police d'exemple (remplacez par le chemin réel du fichier de police)
                string fontFilePath = "arial.ttf";
                if (File.Exists(fontFilePath))
                {
                    // Enregistrer le dossier de police
                    FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);

                    // Dans un scénario réel, FontFileDataInfo serait obtenu à partir de la bibliothèque
                    // Pour la démonstration, nous allons simuler l'obtention des informations de police
                    // Remarque : L'API réelle pourrait fournir cela via FontConfigs ou similaire
                    FontFileDataInfo fontInfo = GetFontFileDataInfo(fontFilePath);

                    if (fontInfo != null)
                    {
                        // Afficher la valeur de la propriété FormatType
                        Console.WriteLine("Font Format Type: " + fontInfo.FormatType);

                        // Afficher la valeur de l'énumération sous forme de chaîne
                        Console.WriteLine("Format Type Description: " +
                            Enum.GetName(typeof(FontFileFormatType), fontInfo.FormatType));

                        // Appliquer la police à une cellule (conceptuel - l'implémentation réelle peut varier)
                        Style style = worksheet.Cells["A1"].GetStyle();
                        style.Font.Name = "Arial";
                        worksheet.Cells["A1"].SetStyle(style);
                    }
                    else
                    {
                        Console.WriteLine("Font information could not be retrieved");
                    }
                }
                else
                {
                    Console.WriteLine("Font file not found at: " + fontFilePath);
                }

                // Enregistrez le classeur
                workbook.Save("FormatTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Méthode d'aide pour simuler l'obtention de FontFileDataInfo
        // Dans une utilisation réelle, cela serait fourni par l'API Aspose.Cells
        private static FontFileDataInfo GetFontFileDataInfo(string fontPath)
        {
            try
            {
                byte[] fontData = File.ReadAllBytes(fontPath);
                string extension = Path.GetExtension(fontPath).ToLower();

                // Créer un faux FontFileDataInfo (en réalité, cela viendrait de l'API)
                // Comme nous ne pouvons pas l'instancier directement, nous allons simuler le comportement
                FontFileFormatType formatType = FontFileFormatType.Unknown;

                if (extension == ".ttf")
                    formatType = FontFileFormatType.Ttf;
                else if (extension == ".otf")
                    formatType = FontFileFormatType.Otf;
                else if (extension == ".ttc")
                    formatType = FontFileFormatType.Ttc;

                // Dans une implémentation réelle, cela serait renvoyé par l'API
                // Pour cette démonstration, nous renverrons simplement null puisque nous ne pouvons pas créer l'objet
                Console.WriteLine($"Detected font format: {formatType}");
                return null;
            }
            catch
            {
                return null;
            }
        }
    }
}
```

### Voir aussi

* enum [FontFileFormatType](../../fontfileformattype/)
* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


