---
title: "Schnittstelle LightCellsDataProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Schnittstelle Aspose.Cells.LightCellsDataProvider. Stellt einen Datenanbieter zum Speichern großer Tabellenkalkulationsdateien im Leichtgewichtsmodus dar."
type: docs
url: /de/net/aspose.cells/lightcellsdataprovider/
---
## LightCellsDataProvider interface

Stellt den Datenanbieter zum Speichern großer Tabellenkalkulationsdateien im Leichtgewichtmodus dar.

```csharp
public interface LightCellsDataProvider
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [IsGatherString](../../aspose.cells/lightcellsdataprovider/isgatherstring/)() | Überprüft, ob der aktuelle Zeichenkettenwert der Zelle in einen globalen Pool aufgenommen werden muss. |
| [NextCell](../../aspose.cells/lightcellsdataprovider/nextcell/)() | Ermittelt die nächste zu speichernde Zelle. |
| [NextRow](../../aspose.cells/lightcellsdataprovider/nextrow/)() | Ermittelt die nächste zu speichernde Zeile. |
| [StartCell](../../aspose.cells/lightcellsdataprovider/startcell/)(Cell) | Beginnt, Daten einer Zelle zu speichern. |
| [StartRow](../../aspose.cells/lightcellsdataprovider/startrow/)(Row) | Beginnt, Daten einer Zeile zu speichern. |
| [StartSheet](../../aspose.cells/lightcellsdataprovider/startsheet/)(int) | Beginnt, ein Arbeitsblatt zu speichern. |

### Hinweise

Beim Speichern einer Arbeitsmappe mit diesem Modus wird [`StartSheet`](./startsheet/) bei jedem Speichern eines Arbeitsblatts in der Arbeitsmappe geprüft. Für ein Blatt, wenn [`StartSheet`](./startsheet/) true zurückgibt, werden alle zu speichernden Daten und Eigenschaften für Zeilen/Zellen dieses Blatts von der Implementierung dieses Interfaces bereitgestellt. Zunächst wird [`NextRow`](./nextrow/) aufgerufen, um den nächsten Zeilenindex zu erhalten, der gespeichert werden soll. Wenn ein gültiger Zeilenindex zurückgegeben wird (der Zeilenindex muss für die zu speichernden Zeilen in aufsteigender Reihenfolge sein), wird ein Row‑Objekt, das diese Zeile repräsentiert, von [`StartRow`](./startrow/) bereitgestellt, damit die Implementierung seine Eigenschaften setzen kann. Für eine Zeile wird [`NextCell`](./nextcell/) zuerst geprüft. Wenn ein gültiger Spaltenindex zurückgegeben wird (der Spaltenindex muss für alle Zellen der aktuellen Zeile in aufsteigender Reihenfolge sein), wird ein Cell‑Objekt, das diese Zelle repräsentiert, von [`StartCell`](./startcell/) bereitgestellt, damit die Implementierung ihre Daten und Eigenschaften setzen kann. Nach [`StartCell`](./startcell/) wird die Zelle direkt in die resultierende Tabellendatei gespeichert. Dann wird die nächste Zelle geprüft und verarbeitet. Bitte beachten Sie, dass der Benutzer nur Werte und Eigenschaften für das aktuelle Row/Cell‑Objekt, das von der entsprechenden Methode bereitgestellt wird, aktualisieren sollte. Da die Zellen­daten in Streaming‑Manier in die Ergebnisdatei geschrieben werden, können die meisten anderen Objekte bereits in die Ergebnisdatei geschrieben worden sein oder es wurden globale Daten für sie gesammelt und geschrieben. Wenn der Benutzer also andere Objekte aktualisiert, während Zellen­daten gespeichert werden, können diese Vorgänge die gespeicherten Daten möglicherweise nicht beeinflussen. Noch schlimmer kann es dazu führen, dass inkonsistente Daten in die Ergebnisdatei gespeichert werden und die Datei schließlich beschädigt wird. Daher sollten für alle anderen Objekte wie Formen, Spaltenbreiten und Stile, bedingte Formatierungen usw. keine Operationen in Methoden dieser Implementierung durchgeführt werden. Stattdessen sollten Sie diese verwalten und vor dem Aufruf der "Save"‑Methode der Arbeitsmappe in den endgültigen Zustand bringen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderDemo
    {
        public static void LightCellsDataProviderExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle einen benutzerdefinierten LightCellsDataProvider
            CustomLightCellsDataProvider dataProvider = new CustomLightCellsDataProvider();

            // Setze den LightCellsDataProvider zum Speichern der Arbeitsmappe
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx)
            {
                LightCellsDataProvider = dataProvider
            };

            // Speichere die Arbeitsmappe mit dem benutzerdefinierten LightCellsDataProvider
            workbook.Save("LightCellsDataProviderExample.xlsx", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;

        public bool StartSheet(int sheetIndex)
        {
            // Beginne mit der Verarbeitung des ersten Blatts
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            // Gehe zur nächsten Zeile
            currentRow++;
            currentCell = -1;

            // Gib den aktuellen Zeilenindex zurück oder -1, wenn keine weiteren Zeilen vorhanden sind
            return currentRow < 10 ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // Initialisiere die Zeile bei Bedarf
        }

        public int NextCell()
        {
            // Gehe zur nächsten Zelle
            currentCell++;

            // Gib den aktuellen Zellenindex zurück oder -1, wenn keine weiteren Zellen vorhanden sind
            return currentCell < 10 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            // Setzen Sie den Wert der Zelle
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            // Gib zurück, ob Zeichenketten in einen globalen Pool gesammelt werden sollen
            return false;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


