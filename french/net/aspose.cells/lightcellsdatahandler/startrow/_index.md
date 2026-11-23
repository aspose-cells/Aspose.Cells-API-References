---
title: "LightCellsDataHandler.StartRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode LightCellsDataHandler. Prépare le traitement d'une ligne"
type: docs
url: /fr/net/aspose.cells/lightcellsdatahandler/startrow/
---
## LightCellsDataHandler.StartRow method

Prépare le traitement d’une ligne.

```csharp
public bool StartRow(int rowIndex)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | l'indice de la prochaine ligne à traiter |

### Valeur de retour

si cette ligne (propriétés ou données des cellules) doit être traitée. false pour ignorer cette ligne et ses cellules et vérifier la ligne suivante.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerMethodStartRowWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                using (Workbook workbook = new Workbook())
                {
                    Worksheet sheet = workbook.Worksheets[0];
                    for (int i = 0; i < 5; i++)
                    {
                        sheet.Cells[i, 0].Value = $"Row {i + 1}";
                    }
                    workbook.Save("input.xlsx");
                }

                LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
                loadOptions.LightCellsDataHandler = new CustomLightCellsDataHandler();
                
                using (Workbook workbook = new Workbook("input.xlsx", loadOptions))
                {
                    workbook.Save("output.xlsx");
                }

                Console.WriteLine("Method executed successfully. Rows with even indices processed.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartRow: {ex.Message}");
            }
        }

        private class CustomLightCellsDataHandler : LightCellsDataHandler
        {
            public bool StartRow(int rowIndex)
            {
                return rowIndex % 2 == 0;
            }

            public bool StartSheet(Worksheet sheet) => true;
            public bool ProcessRow(Row row) => true;
            public bool StartCell(int columnIndex) => true;
            public bool ProcessCell(Cell cell) => true;
        }
    }
}
```

### Voir aussi

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


