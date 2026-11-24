---
title: "Schnittstelle LightCellsDataHandler"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.LightCellsDataHandler‑Schnittstelle. Stellt einen Zellen‑Daten‑Handler zum Lesen großer Tabellendateien im Leichtgewichtmodus dar."
type: docs
url: /de/net/aspose.cells/lightcellsdatahandler/
---
## LightCellsDataHandler interface

Stellt den Zellen‑Datenhandler zum Lesen großer Tabellenkalkulationsdateien im Leichtgewichtmodus dar.

```csharp
public interface LightCellsDataHandler
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ProcessCell](../../aspose.cells/lightcellsdatahandler/processcell/)(Cell) | Beginnt mit der Verarbeitung einer Zelle. |
| [ProcessRow](../../aspose.cells/lightcellsdatahandler/processrow/)(Row) | Beginnt mit der Verarbeitung einer Zeile. |
| [StartCell](../../aspose.cells/lightcellsdatahandler/startcell/)(int) | Bereitet die Verarbeitung einer Zelle vor. |
| [StartRow](../../aspose.cells/lightcellsdatahandler/startrow/)(int) | Bereitet die Verarbeitung einer Zeile vor. |
| [StartSheet](../../aspose.cells/lightcellsdatahandler/startsheet/)(Worksheet) | Beginnt mit der Verarbeitung eines Arbeitsblatts. |

### Hinweise

Beim Lesen einer Arbeitsmappe in diesem Modus wird [`StartSheet`](./startsheet/) bei jedem Lesen eines Arbeitsblatts in der Arbeitsmappe überprüft. Für ein Blatt, wenn [`StartSheet`](./startsheet/) true zurückgibt, werden alle Daten und Eigenschaften von Zeilen/Zellen dieses Blatts von der Implementierung dieser Schnittstelle geprüft und verarbeitet. Für jede Zeile wird [`StartRow`](./startrow/) aufgerufen, um zu prüfen, ob sie verarbeitet werden muss. Wenn eine Zeile verarbeitet werden muss, werden zunächst die Eigenschaften dieser Zeile gelesen und der Benutzer kann über [`ProcessRow`](./processrow/) auf ihre Eigenschaften zugreifen. Wenn die Zellen der Zeile ebenfalls verarbeitet werden müssen, sollte [`ProcessRow`](./processrow/) true zurückgeben und anschließend wird [`StartCell`](./startcell/) für jede vorhandene Zelle in dieser Zeile aufgerufen, um zu prüfen, ob eine Zelle verarbeitet werden muss. Wenn eine Zelle verarbeitet werden muss, wird [`ProcessCell`](./processcell/) von der Implementierung dieser Schnittstelle aufgerufen, um die Zelle zu verarbeiten. Bitte beachten Sie, dass der Benutzer nur mit den Werten und Eigenschaften des aktuellen Zeilen-/Zellobjekts arbeiten sollte, das von der jeweiligen Methode bereitgestellt wird. Da die Zellen­daten aus der Vorlagendatei in Streaming‑Verfahren gelesen werden, können die meisten anderen Objekte später nach dem Laden der Zellen­daten zurückgesetzt/aktualisiert werden. Wenn der Benutzer also in dieser Implementierung andere Objekte manipuliert, können diese Vorgänge die im Arbeitsbuch vorhandenen Objekte möglicherweise nicht beeinflussen. Oder noch schlimmer, diese Vorgänge können inkonsistente Daten im Arbeitsbuch erzeugen und später unerwartete Probleme oder Ausnahmen verursachen. Daher sollten Sie für alle anderen Objekte wie Formen, Spaltenbreiten und Stile, bedingte Formatierungen usw. in keinen Methoden dieser Implementierung an ihnen arbeiten. Stattdessen verwalten Sie sie bitte, nachdem das Arbeitsbuch erstellt wurde.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerDemo : LightCellsDataHandler
    {
        public static void LightCellsDataHandlerExample()
        {
            // Erstelle eine Arbeitsmappe und lade sie mit LightCellsDataHandler
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine Instanz von LightCellsDataHandlerDemo
            LightCellsDataHandlerDemo handler = new LightCellsDataHandlerDemo();

            // Setzen Sie den LightCellsDataHandler für die Arbeitsmappe
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = handler;

            // Lade die Arbeitsmappe mit den angegebenen Ladeoptionen
            workbook = new Workbook("LargeFile_original.xlsx", loadOptions);

            // Speichern Sie die Arbeitsmappe, um den Vorgang zu demonstrieren
            workbook.Save("ProcessedLargeFile.xlsx");
        }

        // Implementieren Sie die Methode StartSheet
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine("Starting to process sheet: " + sheet.Name);
            return true; // Continue processing
        }

        // Implementieren Sie die Methode StartRow
        public bool StartRow(int rowIndex)
        {
            Console.WriteLine("Starting to process row: " + rowIndex);
            return true; // Continue processing
        }

        // Implementieren Sie die Methode ProcessRow
        public bool ProcessRow(Row row)
        {
            Console.WriteLine("Processing row: " + row.Index);
            return true; // Continue processing
        }

        // Implementieren Sie die Methode StartCell
        public bool StartCell(int columnIndex)
        {
            Console.WriteLine("Starting to process cell in column: " + columnIndex);
            return true; // Continue processing
        }

        // Implementieren Sie die Methode ProcessCell
        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine("Processing cell: " + cell.Name + " with value: " + cell.StringValue);
            return true; // Continue processing
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


