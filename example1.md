# Example code to display a message:
### You can include this in main.py  or just type it from a REPL prompt.

```python
import CHAR_LCD as lcd

lcd.init_pins('Y9','Y10')

lcd.reset_display()
# A second reset is sometimes necessary.
lcd.reset_display() 
lcd.clear_display()

#Tell the module how big our display is.
# E.g.  2x16  or  4x20
lcd.init_size(4,20)

#Locate cursor and write a character.
lcd.locate(2,5)
lcd.write_character(0x23)

#Write a line of text.
lcd.write_line(3,'Hello world.')
lcd.write_line(4,'Much LCD enjoyment.')
 
```
