##set_header method
## set_header(self, section, header_script) {#int-System.String}
Sets a script formatting the header of an Excel file.
```python
def set_header(self, section, header_script):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| header_script | System.String | Header format script. |
### Remarks
Script commands:
| Command | Description |
| :- | :- |
| &P| Current page number　 |
| &N| Page count　 |
| &D| Current date　 |
| &T| Current time |
| &A| Sheet name |
| &F| File name without path |
| &"<FontName>"| Font name, for example: &"Arial" |
| &"<FontName>, <FontStyle>"| Font name and font style, for example: &"Arial,Bold" |
| &<FontSize>| Font size. If this command is followed by a plain number to be printed in the header, it will be separated from the font height with a space character. |
| &K<RRGGBB>| Font color, for example(RED): &KFF0000 |
| &G| Image script |
For example: "&Arial,Bold&8Header Note"
### See Also
* module [`aspose.cells`](../../)
* class [`PageSetup`](/cells/python-net/aspose.cells/pagesetup)
