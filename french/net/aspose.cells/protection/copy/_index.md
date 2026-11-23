---
title: "Protection.Copy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Protection. Copie les informations de protection"
type: docs
url: /fr/net/aspose.cells/protection/copy/
---
## Protection.Copy method

Copier les informations de protection.

```csharp
public void Copy(Protection source)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Protection |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionMethodCopyWithProtectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer les paramètres de protection source - utiliser la protection existante de la feuille
            Protection sourceProtection = worksheet.Protection;
            sourceProtection.AllowDeletingColumn = true;
            sourceProtection.AllowInsertingRow = false;
            sourceProtection.Password = "test123";
            sourceProtection.AllowFormattingCell = true;

            // Obtenir les paramètres de protection cibles
            Protection targetProtection = worksheet.Protection;

            try
            {
                // Appeler la méthode Copy avec le paramètre Protection
                targetProtection.Copy(sourceProtection);

                Console.WriteLine("Protection settings copied successfully.");
                Console.WriteLine($"Target protection - AllowDeletingColumn: {targetProtection.AllowDeletingColumn}");
                Console.WriteLine($"Target protection - AllowInsertingRow: {targetProtection.AllowInsertingRow}");
                Console.WriteLine($"Target protection - Password set: {!string.IsNullOrEmpty(targetProtection.Password)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error copying protection settings: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("ProtectionCopyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


