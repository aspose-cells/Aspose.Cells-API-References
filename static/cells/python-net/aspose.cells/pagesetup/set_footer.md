##set_footer method
## set_footer(self, section, footer_script) {#int-System.String}
Sets a script formatting the footer of an Excel file.
```python
def set_footer(self, section, footer_script):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| section | int | 0: Left Section, 1: Center Section, 2: Right Section. |
| footer_script | System.String | Footer format script. |
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
For example: "&Arial,Bold&8Footer Note"
### See Also
* module [`aspose.cells`](../../)
* class [`PageSetup`](/cells/python-net/aspose.cells/pagesetup)
