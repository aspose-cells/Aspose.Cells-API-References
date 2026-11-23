---
title: "Workbook.SetEncryptionOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Définir les options de chiffrement"
type: docs
url: /fr/net/aspose.cells/workbook/setencryptionoptions/
---
## Workbook.SetEncryptionOptions method

Définir les options de chiffrement.

```csharp
public void SetEncryptionOptions(EncryptionType encryptionType, int keyLength)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| encryptionType | EncryptionType | Le type de chiffrement. |
| keyLength | Int32 | La longueur de la clé. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetEncryptionOptionsWithEncryptionTypeInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter des données à la feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Encryption");
            
            // Définir le mot de passe et les options de chiffrement
            workbook.Settings.Password = "1234";
            workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
            
            // Enregistrez le classeur chiffré
            workbook.Save("EncryptedWorkbook.xls", SaveFormat.Excel97To2003);
            
            // Vérifiez en chargeant le classeur chiffré
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "1234";
            Workbook encryptedWorkbook = new Workbook("EncryptedWorkbook.xls", loadOptions);
            
            Console.WriteLine("Workbook encrypted and loaded successfully.");
        }
    }
}
```

### Voir aussi

* enum [EncryptionType](../../encryptiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


