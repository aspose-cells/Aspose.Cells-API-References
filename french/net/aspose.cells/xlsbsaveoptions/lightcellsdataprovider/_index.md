---
title: "XlsbSaveOptions.LightCellsDataProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XlsbSaveOptions. Le fournisseur de données pour enregistrer le classeur en mode léger"
type: docs
url: /fr/net/aspose.cells/xlsbsaveoptions/lightcellsdataprovider/
---
## XlsbSaveOptions.LightCellsDataProvider property

Le fournisseur de données pour enregistrer le classeur en mode léger.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir des données d'exemple
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Data {i}");
            }

            // Créer des options d’enregistrement XLSB
            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            // Enregistrer le classeur avec LightCellsDataProvider
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Vérifier les données enregistrées
                stream.Seek(0, SeekOrigin.Begin);
                Workbook savedWorkbook = new Workbook(stream);
                Console.WriteLine("Workbook saved successfully with LightCellsDataProvider");
            }
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        public bool IsGatherString()
        {
            return true;
        }

        public int NextCell()
        {
            // Implémenter la logique d’itération des cellules ici
            return -1; // Return -1 when no more cells
        }

        public int NextRow()
        {
            // Implémenter la logique d’itération des lignes ici
            return -1; // Return -1 when no more rows
        }

        public void StartCell(Cell cell)
        {
            // Implémenter la logique de traitement des cellules ici
        }

        public void StartRow(Row row)
        {
            // Implémenter la logique de traitement des lignes ici
        }

        public bool StartSheet(int sheetIndex)
        {
            // Implémenter la logique de traitement des feuilles ici
            return true; // Return true to process the sheet
        }
    }
}
```

### Voir aussi

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


