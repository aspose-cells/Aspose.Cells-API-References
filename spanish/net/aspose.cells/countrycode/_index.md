---
title: "Enumeración CountryCode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.CountryCode. Representa los identificadores de país de Excel"
type: docs
url: /es/net/aspose.cells/countrycode/
---
## CountryCode enumeration

Representa los identificadores de país de Excel.

```csharp
public enum CountryCode
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Default | `0` |  |
| USA | `1` | Estados Unidos |
| Canada | `2` | Canadá |
| LatinAmeric | `3` | América Latina, excepto Brasil |
| Russia | `7` | Rusia |
| Egypt | `20` | Egipto |
| Greece | `30` | Grecia |
| Netherlands | `31` | Países Bajos |
| Belgium | `32` | Bélgica |
| France | `33` | Francia |
| Spain | `34` | España |
| Hungary | `36` | Hungría |
| Italy | `39` | Italia |
| Switzerland | `41` | Suiza |
| Austria | `43` | Austria |
| UnitedKingdom | `44` | Reino Unido |
| Denmark | `45` | Dinamarca |
| Sweden | `46` | Suecia |
| Norway | `47` | Noruega |
| Poland | `48` | Polonia |
| Germany | `49` | Alemania |
| Mexico | `52` | México |
| Brazil | `55` | Brasil |
| Australia | `61` | Australia |
| NewZealand | `64` | Nueva Zelanda |
| Thailand | `66` | Tailandia |
| Japan | `81` | Japón |
| SouthKorea | `82` | Corea del Sur |
| VietNam | `84` | Vietnam |
| China | `86` | República Popular de China |
| Turkey | `90` | Turquía |
| India | `91` | India |
| Algeria | `213` | Argelia |
| Morocco | `216` | Marruecos |
| Libya | `218` | Libia |
| Portugal | `351` | Portugal |
| Iceland | `354` | Islandia |
| Finland | `358` | Finlandia |
| Czech | `420` | República Checa |
| Taiwan | `886` | Taiwán |
| Lebanon | `961` | Líbano |
| Jordan | `962` | Jordania |
| Syria | `963` | Siria |
| Iraq | `964` | Irak |
| Kuwait | `965` | Kuwait |
| Saudi | `966` | Arabia Saudita |
| UnitedArabEmirates | `971` | Emiratos Árabes Unidos |
| Israel | `972` | Israel |
| Qatar | `974` | Qatar |
| Iran | `981` | Irán |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CountryCodeDemo
    {
        public static void CountryCodeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer el código de país para el libro de trabajo
            workbook.Settings.LanguageCode = CountryCode.USA;
            workbook.Settings.Region = CountryCode.USA;

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells[0, 0].PutValue("Country");
            worksheet.Cells[0, 1].PutValue("Code");

            worksheet.Cells[1, 0].PutValue("United States");
            worksheet.Cells[1, 1].PutValue((int)CountryCode.USA);

            worksheet.Cells[2, 0].PutValue("Canada");
            worksheet.Cells[2, 1].PutValue((int)CountryCode.Canada);

            worksheet.Cells[3, 0].PutValue("France");
            worksheet.Cells[3, 1].PutValue((int)CountryCode.France);

            worksheet.Cells[4, 0].PutValue("Germany");
            worksheet.Cells[4, 1].PutValue((int)CountryCode.Germany);

            // Guarda el libro de trabajo
            workbook.Save("CountryCodeExample.xlsx");
            workbook.Save("CountryCodeExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


