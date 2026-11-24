---
title: "WorkbookSettings.Region"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Liest oder setzt die regionalen Einstellungen für die Arbeitsmappe"
type: docs
url: /de/net/aspose.cells/workbooksettings/region/
---
## WorkbookSettings.Region property

Liest oder setzt die regionalen Einstellungen für die Arbeitsmappe.

```csharp
public CountryCode Region { get; set; }
```

### Hinweise

1. Regionale Einstellungen, die von der Aspose.Cells-Komponente für eine Arbeitsmappe verwendet werden, die aus einer Vorlagendatei geladen wurde: i). Für eine XLS-Datei gibt es Felder, die für regionale Einstellungen definiert sind, und MS Excel speichert regionale Einstellungsdaten beim Speichern der XLS-Datei in der Datei. Daher verwenden wir die in der Vorlagendatei gespeicherte Region für die Arbeitsmappe. Wenn Sie die in der XLS-Datei gespeicherte Region nicht verwenden möchten, setzen Sie sie nach dem Laden der Vorlagendatei auf die gewünschte (z. B. CountryCode.Default) zurück. Und wir speichern den vom Benutzer angegebenen Wert (über diese Methode) ebenfalls beim Speichern einer XLS-Datei in der Datei. ii). Für andere Dateiformate, wie XLSX, XLSB usw., ist im Dateiformatspezifikation kein Feld für regionale Einstellungen definiert. Daher verwenden wir die regionalen Einstellungen der Anwendungsumgebung für die Arbeitsmappe. Und der vom Benutzer angegebene Wert (über diese Methode) kann für die erzeugten Dateien mit diesen Formaten nicht beibehalten werden. 2. Für die Anzeige in MS Excel: Die hier angewendeten regionalen Einstellungen wirken nur zur Laufzeit mit der Aspose.Cells-Komponente und nicht beim Betrachten der erzeugten Datei mit MS Excel. Selbst bei einer erzeugten XLS-Datei, in der die angegebenen regionalen Einstellungsdaten gespeichert wurden, wird beim Betrachten/Bearbeiten mit MS Excel die von MS Excel zur Formatierung verwendete Region stets die standardmäßigen regionalen Einstellungen der Umgebung sein, in der MS Excel ausgeführt wird, nicht die in der Datei gespeicherte. Das ist das Verhalten von MS Excel und kann durch Code nicht geändert werden.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRegionDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.Japan;
            
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(44089); // Represents 2020-09-15
            
            Style style = cell.GetStyle();
            style.Custom = "[$-F800]yyyy年m月d日";
            cell.SetStyle(style);
            
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### Siehe auch

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


