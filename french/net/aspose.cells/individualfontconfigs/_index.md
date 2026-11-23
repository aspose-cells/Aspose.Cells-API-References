---
title: "Classe IndividualFontConfigs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.IndividualFontConfigs. Configurations de police pour chaque objet Workbook"
type: docs
url: /fr/net/aspose.cells/individualfontconfigs/
---
## IndividualFontConfigs class

Configurations de police pour chaque objet [`Workbook`](../workbook/).

```csharp
public class IndividualFontConfigs
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [IndividualFontConfigs](individualfontconfigs/)() | Constructeur. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetFontSources](../../aspose.cells/individualfontconfigs/getfontsources/)() | Obtient une copie du tableau contenant la liste des sources |
| [GetFontSubstitutes](../../aspose.cells/individualfontconfigs/getfontsubstitutes/)(string) | Renvoie un tableau contenant les noms de substituts de police à utiliser si la police d'origine n'est pas présentée. |
| [SetFontFolder](../../aspose.cells/individualfontconfigs/setfontfolder/)(string, bool) | Définit le dossier des polices |
| [SetFontFolders](../../aspose.cells/individualfontconfigs/setfontfolders/)(string[], bool) | Définit les dossiers de police |
| [SetFontSources](../../aspose.cells/individualfontconfigs/setfontsources/)(FontSourceBase[]) | Définit les sources de police. |
| [SetFontSubstitutes](../../aspose.cells/individualfontconfigs/setfontsubstitutes/)(string, string[]) | Définit les noms de substituts de police pour un nom de police d'origine donné. |

### Exemples

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIndividualFontConfigsDemo
    {
        public static void Run()
        {
            // Créer des répertoires temporaires pour les sources de police
            string tempFontFolder1 = Path.Combine(Path.GetTempPath(), "FontFolder1_" + Guid.NewGuid().ToString());
            string tempFontFolder2 = Path.Combine(Path.GetTempPath(), "FontFolder2_" + Guid.NewGuid().ToString());
            Directory.CreateDirectory(tempFontFolder1);
            Directory.CreateDirectory(tempFontFolder2);

            // Créer un fichier CSV d'exemple
            string csvFilePath = "sample_data.csv";
            File.WriteAllText(csvFilePath, "Name,Age\nJohn,30\nAlice,25", Encoding.UTF8);

            try
            {
                // Initialiser la configuration de police
                IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

                // Définir les substituts de police pour Arial
                fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Verdana" });

                // Configurer les répertoires de police
                fontConfigs.SetFontFolder(tempFontFolder1, false);
                fontConfigs.SetFontFolders(new string[] { tempFontFolder1, tempFontFolder2 }, true);

                // Configurer les sources de police
                FontSourceBase[] fontSources = {
                    new FolderFontSource(tempFontFolder1, false),
                    new FolderFontSource(tempFontFolder2, true)
                };
                fontConfigs.SetFontSources(fontSources);

                // Créer des options de chargement de texte avec des configurations de police
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
                {
                    FontConfigs = fontConfigs
                };

                // Charger le classeur avec les options configurées
                using (Workbook workbook = new Workbook(csvFilePath, loadOptions))
                {
                    // Enregistrer en tant que fichier Excel
                    workbook.Save("output_with_font_config.xlsx");
                }
            }
            finally
            {
                // Nettoyer les ressources temporaires
                if (Directory.Exists(tempFontFolder1)) Directory.Delete(tempFontFolder1, true);
                if (Directory.Exists(tempFontFolder2)) Directory.Delete(tempFontFolder2, true);
                if (File.Exists(csvFilePath)) File.Delete(csvFilePath);
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


