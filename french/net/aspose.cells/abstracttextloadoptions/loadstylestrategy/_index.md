---
title: "AbstractTextLoadOptions.LoadStyleStrategy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AbstractTextLoadOptions. Indique la stratégie à appliquer pour le style des valeurs analysées lors de la conversion d’une chaîne en nombre ou en date/heure"
type: docs
url: /fr/net/aspose.cells/abstracttextloadoptions/loadstylestrategy/
---
## AbstractTextLoadOptions.LoadStyleStrategy property

Indique la stratégie à appliquer pour le style des valeurs analysées lors de la conversion d'une chaîne en nombre ou en date/heure.

```csharp
public TxtLoadStyleStrategy LoadStyleStrategy { get; set; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définissez un style personnalisé pour la démonstration
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.Name = "Arial";
            customStyle.Font.Size = 12;
            customStyle.Font.Color = System.Drawing.Color.Blue;
            customStyle.Pattern = BackgroundType.Solid;
            customStyle.ForegroundColor = System.Drawing.Color.LightYellow;

            // Appliquer le style à une cellule
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(customStyle);

            // Créez des données CSV
            string csvData = "Data1,Data2\nValue1,Value2";
            byte[] byteArray = Encoding.ASCII.GetBytes(csvData);
            MemoryStream stream = new MemoryStream(byteArray);

            // Créez des options de chargement de texte avec LoadStyleStrategy
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                LoadStyleStrategy = TxtLoadStyleStrategy.BuiltIn
            };

            // Importez les données CSV avec les options de chargement spécifiées
            cells.ImportCSV(stream, loadOptions, 0, 0);

            // Enregistrer le classeur pour démontrer le résultat
            workbook.Save("LoadStyleStrategyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [TxtLoadStyleStrategy](../../txtloadstylestrategy/)
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


