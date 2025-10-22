##ControlMatchEntryType
Represents how a ListBox or ComboBox searches its list as the user types.
## ControlMatchEntryType enumeration
Represents how a ListBox or ComboBox searches its list as the user types.
### Values
| Name | Value | Description |
| --- | --- | --- |
| FirstLetter | `0` | The control searches for the next entry that starts with the character entered. Repeatedly typing the same letter cycles through all entries beginning with that letter. |
| Complete | `1` | As each character is typed, the control searches for an entry matching all characters entered. |
| None | `2` | The list will not be searched when characters are typed. |
