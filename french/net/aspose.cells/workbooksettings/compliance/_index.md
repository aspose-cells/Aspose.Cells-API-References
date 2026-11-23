---
title: "WorkbookSettings.Compliance"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Spécifie la version OOXML du document de sortie. La valeur par défaut est Ecma376_2006"
type: docs
url: /fr/net/aspose.cells/workbooksettings/compliance/
---
## WorkbookSettings.Compliance property

Spécifie la version OOXML du document de sortie. La valeur par défaut est Ecma376_2006.

```csharp
public OoxmlCompliance Compliance { get; set; }
```

### Remarques

Uniquement pour les fichiers .xlsx.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyComplianceDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorkbookSettings settings = workbook.Settings;
            
            // Définir la conformité en mode strict
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;
            
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Strict Compliance Demo");
            
            workbook.Save("WorkbookComplianceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [OoxmlCompliance](../../ooxmlcompliance/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


