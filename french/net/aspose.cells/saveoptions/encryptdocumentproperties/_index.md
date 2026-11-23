---
title: "SaveOptions.EncryptDocumentProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SaveOptions. Indique s’il faut chiffrer les propriétés du document lors de l’enregistrement au format .xls. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/saveoptions/encryptdocumentproperties/
---
## SaveOptions.EncryptDocumentProperties property

Indique s'il faut chiffrer les propriétés du document lors de l'enregistrement au format .xls. La valeur par défaut est vraie.

```csharp
public bool EncryptDocumentProperties { get; set; }
```

### Remarques

Uniquement pour les fichiers .xls, .xlsx, .xlsb et .xlsm.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyEncryptDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir certaines propriétés du document
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Définir la protection par mot de passe
            workbook.Settings.Password = "password123";
            
            // Enregistrer avec EncryptDocumentProperties = true (par défaut)
            XlsSaveOptions saveOptions1 = new XlsSaveOptions();
            saveOptions1.EncryptDocumentProperties = true;
            workbook.Save("encrypted_properties.xls", saveOptions1);
            
            // Enregistrer avec EncryptDocumentProperties = false
            XlsSaveOptions saveOptions2 = new XlsSaveOptions();
            saveOptions2.EncryptDocumentProperties = false;
            workbook.Save("unencrypted_properties.xls", saveOptions2);
            
            // Vérifier en rechargeant
            Console.WriteLine("Files saved. Try opening them to see the difference in property encryption.");
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


