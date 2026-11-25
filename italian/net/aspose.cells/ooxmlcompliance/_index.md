---
title: "Enum OoxmlCompliance"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.OoxmlCompliance enum. Consente di specificare quale specifica OOXML verrà utilizzata durante il salvataggio nel formato Xlsx"
type: docs
url: /it/net/aspose.cells/ooxmlcompliance/
---
## OoxmlCompliance enumeration

Consente di specificare quale specifica OOXML verrà utilizzata durante il salvataggio nel formato Xlsx.

```csharp
public enum OoxmlCompliance
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Ecma376_2006 | `0` | ECMA-376 1ª Edizione, 2006. |
| Iso29500_2008_Strict | `1` | Livello di conformità Strict ISO/IEC 29500:2008. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlComplianceDemo
    {
        public static void OoxmlComplianceExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Imposta il livello di conformità OOXML a ISO/IEC 29500:2008 Strict
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;

            // Aggiungi alcuni dati al worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, World!");

            // Salva la cartella di lavoro con il livello di conformità OOXML specificato
            workbook.Save("OoxmlComplianceExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


