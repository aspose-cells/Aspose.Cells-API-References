---
title: "XmlSaveOptions.XmlSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur XmlSaveOptions. Crée des options pour l'enregistrement d'un fichier xml"
type: docs
url: /fr/net/aspose.cells/xmlsaveoptions/xmlsaveoptions/
---
## XmlSaveOptions constructor

Crée des options pour l'enregistrement d'un fichier XML.

```csharp
public XmlSaveOptions()
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des données de test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(63);

            // Première démonstration : Enregistrer en XML avec SheetNameAsElementName
            XmlSaveOptions saveOptions1 = new XmlSaveOptions();
            saveOptions1.SheetNameAsElementName = true;
            workbook.Save("output1.xml", saveOptions1);
            
            // Deuxième démonstration : Enregistrer en XML avec SheetNameAsElementName et DataAsAttribute
            XmlSaveOptions saveOptions2 = new XmlSaveOptions();
            saveOptions2.SheetNameAsElementName = true;
            saveOptions2.DataAsAttribute = true;
            workbook.Save("output2.xml", saveOptions2);

            Console.WriteLine("XML files created successfully.");
        }
    }
}
```

### Voir aussi

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


