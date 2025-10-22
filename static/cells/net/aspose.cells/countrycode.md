##Enum CountryCode
Aspose.Cells.CountryCode enum. Represents Excel country identifiers
## CountryCode enumeration
Represents Excel country identifiers.
```csharp
public enum CountryCode
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `0` |  |
| USA | `1` | United States |
| Canada | `2` | Canada |
| LatinAmeric | `3` | Latin America, except Brazil |
| Russia | `7` | Russia |
| Egypt | `20` | Egypt |
| Greece | `30` | Greece |
| Netherlands | `31` | Netherlands |
| Belgium | `32` | Belgium |
| France | `33` | France |
| Spain | `34` | Spain |
| Hungary | `36` | Hungary |
| Italy | `39` | Italy |
| Switzerland | `41` | Switzerland |
| Austria | `43` | Austria |
| UnitedKingdom | `44` | United Kingdom |
| Denmark | `45` | Denmark |
| Sweden | `46` | Sweden |
| Norway | `47` | Norway |
| Poland | `48` | Poland |
| Germany | `49` | Germany |
| Mexico | `52` | Mexico |
| Brazil | `55` | Brazil |
| Australia | `61` | Australia |
| NewZealand | `64` | New Zealand |
| Thailand | `66` | Thailand |
| Japan | `81` | Japan |
| SouthKorea | `82` | SouthKorea |
| VietNam | `84` | Viet Nam |
| China | `86` | People's Republic of China |
| Turkey | `90` | Turkey |
| India | `91` | India |
| Algeria | `213` | Algeria |
| Morocco | `216` | Morocco |
| Libya | `218` | Libya |
| Portugal | `351` | Portugal |
| Iceland | `354` | Iceland |
| Finland | `358` | Finland |
| Czech | `420` | Czech Republic |
| Taiwan | `886` | Taiwan |
| Lebanon | `961` | Lebanon |
| Jordan | `962` | Jordan |
| Syria | `963` | Syria |
| Iraq | `964` | Iraq |
| Kuwait | `965` | Kuwait |
| Saudi | `966` | Saudi Arabia |
| UnitedArabEmirates | `971` | United Arab Emirates |
| Israel | `972` | Israel |
| Qatar | `974` | Qatar |
| Iran | `981` | Iran |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CountryCodeDemo
{
public static void CountryCodeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set the country code for the workbook
workbook.Settings.LanguageCode = CountryCode.USA;
workbook.Settings.Region = CountryCode.USA;
// Add some data to the worksheet
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
// Save the workbook
workbook.Save("CountryCodeExample.xlsx");
workbook.Save("CountryCodeExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
