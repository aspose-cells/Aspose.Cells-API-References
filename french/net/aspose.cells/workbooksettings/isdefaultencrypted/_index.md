---
title: "WorkbookSettings.IsDefaultEncrypted"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Indique si le classeur est chiffré avec le mot de passe par défaut lorsque la structure et les fenêtres du classeur sont verrouillées"
type: docs
url: /fr/net/aspose.cells/workbooksettings/isdefaultencrypted/
---
## WorkbookSettings.IsDefaultEncrypted property

Indique si le workbook est chiffré avec le mot de passe par défaut lorsque la Structure et les Fenêtres du workbook sont verrouillées.

```csharp
public bool IsDefaultEncrypted { get; set; }
```

### Remarques

La valeur par défaut est maintenant false. C'est identique à MS Excel 2013.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsDefaultEncryptedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Console.WriteLine("IsDefaultEncrypted: " + workbook.Settings.IsDefaultEncrypted);
            
            workbook.Settings.IsDefaultEncrypted = true;
            Console.WriteLine("After setting to true: " + workbook.Settings.IsDefaultEncrypted);
        }
    }
}
```

### Voir aussi

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


