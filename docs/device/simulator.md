# Simulator

The JavaScript simulator allows you to test and execute most BBC micro:bit programs in the browser.
It allows you to emulate sensor data or user interactions.

```sim
count = 5

display.show(str(count))
if button_a.is_pressed():
	count = count - 1
	display.show(str(count))
if count <=0:
	display.scroll("You Win!!!")
elif button_b.is_pressed():
	count = count - 2
	display.show(str(count))
if count <=0:
	display.scroll("You Win!!!")
elif pin0.is_touched():
	count = count - 3
	display.show(str(count))
if count <=0:
	display.scroll("You Win!!!")
