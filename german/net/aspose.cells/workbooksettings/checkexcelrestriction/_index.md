---
title: "WorkbookSettings.CheckExcelRestriction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt an, ob die Beschränkungen der Excel‑Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht das Eingeben eines Zeichenfolgenwertes, der länger als 32 KB ist. Wenn Sie einen Wert eingeben, der länger als 32 KB ist, etwa über Cell.PutValueString, erhalten Sie bei aktivierter Eigenschaft (true) eine Ausnahme. Ist die Eigenschaft deaktiviert (false), akzeptieren wir Ihren Eingabewert als Zellenwert, sodass Sie später den vollständigen Zeichenfolgenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel‑Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel‑Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel‑Datei kommen."
type: docs
url: /de/net/aspose.cells/workbooksettings/checkexcelrestriction/
---
## WorkbookSettings.CheckExcelRestriction property

Ob die Beschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Beispielsweise erlaubt Excel nicht, einen Zeichenfolgenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K eingeben, etwa mit Cell.PutValue(string), erhalten Sie bei true dieser Eigenschaft eine Exception. Ist die Eigenschaft false, akzeptieren wir Ihren Eingabestring als Zellwert, sodass Sie später den vollständigen Zeichenfolgenwert für andere Dateiformate wie CSV ausgeben können. Wenn Sie jedoch einen Wert festlegen, der für das Excel-Dateiformat ungültig ist, sollten Sie die Arbeitsmappe später nicht im Excel-Format speichern. Andernfalls kann es zu unerwarteten Fehlern in der erzeugten Excel-Datei kommen.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Excel-Beschränkungsprüfung deaktivieren
            workbook.Settings.CheckExcelRestriction = false;
            
            // Fügen Sie eine Zeichenfolge ein, die die normalen Excel‑Grenzen überschreitet
            string longString = new string('a', 40000);
            workbook.Worksheets[0].Cells["A1"].PutValue(longString);
            
            // Speichern und erneut laden, um zu überprüfen, dass die Beschränkung umgangen wurde
            string tempFile = Guid.NewGuid().ToString() + ".txt";
            workbook.Save(tempFile, new TxtSaveOptions());
            
            Workbook loadedWorkbook = new Workbook(tempFile, new LoadOptions { CheckExcelRestriction = false });
            Console.WriteLine("String length: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue.Length);
        }
    }
}
```

### Siehe auch

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


