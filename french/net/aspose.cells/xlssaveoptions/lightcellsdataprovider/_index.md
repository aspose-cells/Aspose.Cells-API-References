---
title: "XlsSaveOptions.LightCellsDataProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété XlsSaveOptions. Le fournisseur de données pour enregistrer le classeur en mode léger"
type: docs
url: /fr/net/aspose.cells/xlssaveoptions/lightcellsdataprovider/
---
## XlsSaveOptions.LightCellsDataProvider property

Le fournisseur de données pour enregistrer le classeur en mode léger.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Créer des options d’enregistrement XLS
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            
            // Définir le LightCellsDataProvider
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();
            
            // Enregistrer le classeur en mode LightCells
            workbook.Save("output.xls", saveOptions);
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
            return 0; // Only process first cell for demonstration
        }

        public int NextRow()
        {
            return 0; // Only process first row for demonstration
        }

        public void StartCell(Cell cell)
        {
            // Définir une valeur de chaîne longue pour démontrer la gestion LightCells
            cell.PutValue(new string('X', 257));
        }

        public void StartRow(Row row)
        {
            // Aucune gestion spéciale des lignes n’est nécessaire pour cette démonstration
        }

        public bool StartSheet(int sheetIndex)
        {
            // Aucune gestion spéciale des feuilles n’est nécessaire pour cette démonstration
            return false;
        }
    }
}
```

### Voir aussi

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


