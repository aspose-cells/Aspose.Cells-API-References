##PaperSizeType Enum
'PaperSizeType enum. Encapsulates the object that represents papersizetype in Go.'
## PaperSizeType Enum
Represents paper size constants.
```go
type PaperSizeType int32
```
## Fields
| Field | Description |
| --- | --- |
|[PaperLetter](./paperletter/) | Letter (8-1/2 in. x 11 in.) |
|[PaperLetterSmall](./paperlettersmall/) | Letter Small (8-1/2 in. x 11 in.) |
|[PaperTabloid](./papertabloid/) | Tabloid (11 in. x 17 in.) |
|[PaperLedger](./paperledger/) | Ledger (17 in. x 11 in.) |
|[PaperLegal](./paperlegal/) | Legal (8-1/2 in. x 14 in.) |
|[PaperStatement](./paperstatement/) | Statement (5-1/2 in. x 8-1/2 in.) |
|[PaperExecutive](./paperexecutive/) | Executive (7-1/4 in. x 10-1/2 in.) |
|[PaperA3](./papera3/) | A3 (297 mm x 420 mm) |
|[PaperA4](./papera4/) | A4 (210 mm x 297 mm) |
|[PaperA4Small](./papera4small/) | A4 Small (210 mm x 297 mm) |
|[PaperA5](./papera5/) | A5 (148 mm x 210 mm) |
|[PaperB4](./paperb4/) | JIS B4 (257 mm x 364 mm) |
|[PaperB5](./paperb5/) | JIS B5 (182 mm x 257 mm) |
|[PaperFolio](./paperfolio/) | Folio (8-1/2 in. x 13 in.) |
|[PaperQuarto](./paperquarto/) | Quarto (215 mm x 275 mm) |
|[Paper10x14](./paper10x14/) | 10 in. x 14 in. |
|[Paper11x17](./paper11x17/) | 11 in. x 17 in. |
|[PaperNote](./papernote/) | Note (8-1/2 in. x 11 in.) |
|[PaperEnvelope9](./paperenvelope9/) | Envelope #9 (3-7/8 in. x 8-7/8 in.) |
|[PaperEnvelope10](./paperenvelope10/) | Envelope #10 (4-1/8 in. x 9-1/2 in.) |
|[PaperEnvelope11](./paperenvelope11/) | Envelope #11 (4-1/2 in. x 10-3/8 in.) |
|[PaperEnvelope12](./paperenvelope12/) | Envelope #12 (4-1/2 in. x 11 in.) |
|[PaperEnvelope14](./paperenvelope14/) | Envelope #14 (5 in. x 11-1/2 in.) |
|[PaperCSheet](./papercsheet/) | C size sheet |
|[PaperDSheet](./paperdsheet/) | D size sheet |
|[PaperESheet](./paperesheet/) | E size sheet |
|[PaperEnvelopeDL](./paperenvelopedl/) | Envelope DL (110 mm x 220 mm) |
|[PaperEnvelopeC5](./paperenvelopec5/) | Envelope C5 (162 mm x 229 mm) |
|[PaperEnvelopeC3](./paperenvelopec3/) | Envelope C3 (324 mm x 458 mm) |
|[PaperEnvelopeC4](./paperenvelopec4/) | Envelope C4 (229 mm x 324 mm) |
|[PaperEnvelopeC6](./paperenvelopec6/) | Envelope C6 (114 mm x 162 mm) |
|[PaperEnvelopeC65](./paperenvelopec65/) | Envelope C65 (114 mm x 229 mm) |
|[PaperEnvelopeB4](./paperenvelopeb4/) | Envelope B4 (250 mm x 353 mm) |
|[PaperEnvelopeB5](./paperenvelopeb5/) | Envelope B5 (176 mm x 250 mm) |
|[PaperEnvelopeB6](./paperenvelopeb6/) | Envelope B6 (176 mm x 125 mm) |
|[PaperEnvelopeItaly](./paperenvelopeitaly/) | Envelope Italy (110 mm x 230 mm) |
|[PaperEnvelopeMonarch](./paperenvelopemonarch/) | Envelope Monarch (3-7/8 in. x 7-1/2 in.) |
|[PaperEnvelopePersonal](./paperenvelopepersonal/) | Envelope (3-5/8 in. x 6-1/2 in.) |
|[PaperFanfoldUS](./paperfanfoldus/) | U.S. Standard Fanfold (14-7/8 in. x 11 in.) |
|[PaperFanfoldStdGerman](./paperfanfoldstdgerman/) | German Standard Fanfold (8-1/2 in. x 12 in.) |
|[PaperFanfoldLegalGerman](./paperfanfoldlegalgerman/) | German Legal Fanfold (8-1/2 in. x 13 in.) |
|[PaperISOB4](./paperisob4/) | B4 (ISO) 250 x 353 mm |
|[PaperJapanesePostcard](./paperjapanesepostcard/) | Japanese Postcard (100mm × 148mm) |
|[Paper9x11](./paper9x11/) | 9? × 11? |
|[Paper10x11](./paper10x11/) | 10? × 11? |
|[Paper15x11](./paper15x11/) | 15? × 11? |
|[PaperEnvelopeInvite](./paperenvelopeinvite/) | Envelope Invite(220mm × 220mm) |
|[PaperLetterExtra](./paperletterextra/) | US Letter Extra 9 \275 x 12 in |
|[PaperLegalExtra](./paperlegalextra/) | US Legal Extra 9 \275 x 15 in |
|[PaperTabloidExtra](./papertabloidextra/) | US Tabloid Extra 11.69 x 18 in |
|[PaperA4Extra](./papera4extra/) | A4 Extra 9.27 x 12.69 in |
|[PaperLetterTransverse](./paperlettertransverse/) | Letter Transverse 8 \275 x 11 in |
|[PaperA4Transverse](./papera4transverse/) | A4 Transverse 210 x 297 mm |
|[PaperLetterExtraTransverse](./paperletterextratransverse/) | Letter Extra Transverse 9\275 x 12 in |
|[PaperSuperA](./papersupera/) | SuperA/SuperA/A4 227 x 356 mm |
|[PaperSuperB](./papersuperb/) | SuperB/SuperB/A3 305 x 487 mm |
|[PaperLetterPlus](./paperletterplus/) | US Letter Plus 8.5 x 12.69 in |
|[PaperA4Plus](./papera4plus/) | A4 Plus 210 x 330 mm |
|[PaperA5Transverse](./papera5transverse/) | A5 Transverse 148 x 210 mm |
|[PaperJISB5Transverse](./paperjisb5transverse/) | B5 (JIS) Transverse 182 x 257 mm |
|[PaperA3Extra](./papera3extra/) | A3 Extra 322 x 445 mm |
|[PaperA5Extra](./papera5extra/) | A5 Extra 174 x 235 mm |
|[PaperISOB5Extra](./paperisob5extra/) | B5 (ISO) Extra 201 x 276 mm |
|[PaperA2](./papera2/) | A2 420 x 594 mm |
|[PaperA3Transverse](./papera3transverse/) | A3 Transverse 297 x 420 mm |
|[PaperA3ExtraTransverse](./papera3extratransverse/) | A3 Extra Transverse 322 x 445 mm |
|[PaperJapaneseDoublePostcard](./paperjapanesedoublepostcard/) | Japanese Double Postcard 200 x 148 mm |
|[PaperA6](./papera6/) | A6 105 x 148 mm |
|[PaperJapaneseEnvelopeKaku2](./paperjapaneseenvelopekaku2/) | Japanese Envelope Kaku #2 |
|[PaperJapaneseEnvelopeKaku3](./paperjapaneseenvelopekaku3/) | Japanese Envelope Kaku #3 |
|[PaperJapaneseEnvelopeChou3](./paperjapaneseenvelopechou3/) | Japanese Envelope Chou #3 |
|[PaperJapaneseEnvelopeChou4](./paperjapaneseenvelopechou4/) | Japanese Envelope Chou #4 |
|[PaperLetterRotated](./paperletterrotated/) | 11in × 8.5in |
|[PaperA3Rotated](./papera3rotated/) | 420mm × 297mm |
|[PaperA4Rotated](./papera4rotated/) | 297mm × 210mm |
|[PaperA5Rotated](./papera5rotated/) | 210mm × 148mm |
|[PaperJISB4Rotated](./paperjisb4rotated/) | B4 (JIS) Rotated 364 x 257 mm |
|[PaperJISB5Rotated](./paperjisb5rotated/) | B5 (JIS) Rotated 257 x 182 mm |
|[PaperJapanesePostcardRotated](./paperjapanesepostcardrotated/) | Japanese Postcard Rotated 148 x 100 mm |
|[PaperJapaneseDoublePostcardRotated](./paperjapanesedoublepostcardrotated/) | Double Japanese Postcard Rotated 148 x 200 mm |
|[PaperA6Rotated](./papera6rotated/) | A6 Rotated 148 x 105 mm |
|[PaperJapaneseEnvelopeKaku2Rotated](./paperjapaneseenvelopekaku2rotated/) | Japanese Envelope Kaku #2 Rotated |
|[PaperJapaneseEnvelopeKaku3Rotated](./paperjapaneseenvelopekaku3rotated/) | Japanese Envelope Kaku #3 Rotated |
|[PaperJapaneseEnvelopeChou3Rotated](./paperjapaneseenvelopechou3rotated/) | Japanese Envelope Chou #3 Rotated |
|[PaperJapaneseEnvelopeChou4Rotated](./paperjapaneseenvelopechou4rotated/) | Japanese Envelope Chou #4 Rotated |
|[PaperJISB6](./paperjisb6/) | B6 (JIS) 128 x 182 mm |
|[PaperJISB6Rotated](./paperjisb6rotated/) | B6 (JIS) Rotated 182 x 128 mm |
|[Paper12x11](./paper12x11/) | 12 x 11 in |
|[PaperJapaneseEnvelopeYou4](./paperjapaneseenvelopeyou4/) | Japanese Envelope You #4 |
|[PaperJapaneseEnvelopeYou4Rotated](./paperjapaneseenvelopeyou4rotated/) | Japanese Envelope You #4 Rotated |
|[PaperPRC16K](./paperprc16k/) | PRC 16K 146 x 215 mm |
|[PaperPRC32K](./paperprc32k/) | PRC 32K 97 x 151 mm |
|[PaperPRCBig32K](./paperprcbig32k/) | PRC 32K(Big) 97 x 151 mm |
|[PaperPRCEnvelope1](./paperprcenvelope1/) | PRC Envelope #1 102 x 165 mm |
|[PaperPRCEnvelope2](./paperprcenvelope2/) | PRC Envelope #2 102 x 176 mm |
|[PaperPRCEnvelope3](./paperprcenvelope3/) | PRC Envelope #3 125 x 176 mm |
|[PaperPRCEnvelope4](./paperprcenvelope4/) | PRC Envelope #4 110 x 208 mm |
|[PaperPRCEnvelope5](./paperprcenvelope5/) | PRC Envelope #5 110 x 220 mm |
|[PaperPRCEnvelope6](./paperprcenvelope6/) | PRC Envelope #6 120 x 230 mm |
|[PaperPRCEnvelope7](./paperprcenvelope7/) | PRC Envelope #7 160 x 230 mm |
|[PaperPRCEnvelope8](./paperprcenvelope8/) | PRC Envelope #8 120 x 309 mm |
|[PaperPRCEnvelope9](./paperprcenvelope9/) | PRC Envelope #9 229 x 324 mm |
|[PaperPRCEnvelope10](./paperprcenvelope10/) | PRC Envelope #10 324 x 458 mm |
|[PaperPRC16KRotated](./paperprc16krotated/) | PRC 16K Rotated |
|[PaperPRC32KRotated](./paperprc32krotated/) | PRC 32K Rotated |
|[PaperPRCBig32KRotated](./paperprcbig32krotated/) | PRC 32K(Big) Rotated |
|[PaperPRCEnvelope1Rotated](./paperprcenvelope1rotated/) | PRC Envelope #1 Rotated 165 x 102 mm |
|[PaperPRCEnvelope2Rotated](./paperprcenvelope2rotated/) | PRC Envelope #2 Rotated 176 x 102 mm |
|[PaperPRCEnvelope3Rotated](./paperprcenvelope3rotated/) | PRC Envelope #3 Rotated 176 x 125 mm |
|[PaperPRCEnvelope4Rotated](./paperprcenvelope4rotated/) | PRC Envelope #4 Rotated 208 x 110 mm |
|[PaperPRCEnvelope5Rotated](./paperprcenvelope5rotated/) | PRC Envelope #5 Rotated 220 x 110 mm |
|[PaperPRCEnvelope6Rotated](./paperprcenvelope6rotated/) | PRC Envelope #6 Rotated 230 x 120 mm |
|[PaperPRCEnvelope7Rotated](./paperprcenvelope7rotated/) | PRC Envelope #7 Rotated 230 x 160 mm |
|[PaperPRCEnvelope8Rotated](./paperprcenvelope8rotated/) | PRC Envelope #8 Rotated 309 x 120 mm |
|[PaperPRCEnvelope9Rotated](./paperprcenvelope9rotated/) | PRC Envelope #9 Rotated 324 x 229 mm |
|[PaperPRCEnvelope10Rotated](./paperprcenvelope10rotated/) | PRC Envelope #10 Rotated 458 x 324 mm |
|[PaperB3](./paperb3/) | usual B3(13.9 x 19.7 in) |
|[PaperBusinessCard](./paperbusinesscard/) | Business Card(90mm x 55 mm) |
|[PaperThermal](./paperthermal/) | Thermal(3 x 11 in) |
|[Custom](./custom/) | Represents the custom paper size. |
