# Action Event Class

**An Action Event is generated when:**

a button is pressed.

a list item is double clicked.

menu item is clicked.

**Constructor**

ActionEvent(Object src, int type, String cmd)

ActionEvent(Object src, int type, String cmd, int modifiers)

ActionEvent(Object src, int type, String cmd, long when, int modifiers)

Here,

src = reference to the object that generated this event.

type = Determine type of event

cmd = command string

modifier = indicates modifier keys (ALT, CTRL, SHIFT); values are ALT_MASK, CTRL_MASK, SHIFT_MASK

when = specifies when the event occured

We can obtain the command name for the envoking ActionEvent object by using: String getActionCommand()

For eg:

When a button is pressed, an action event is generated that has a command name equal to the label on that button.

**Other Methods **:

int getModifier()

long getWhen()

**KeyEvent Class**
It is generated when:

Keyboard input occurs

**Types of KeyEvent**

KEY_PRESSED - generated when key is pressed.

KEY_RELEASED - generated when key is released.

KEY_TYPED - generated when key is generated.

Constants

VK_ALT, VK_DOWN, VK_LEFT, VK_RIGHT, VK_ENTER, VK_ESCAPE, VK_CONTROL, VK_SHIFT,

**Methods**

char getKeyChar ();

int getKeyChar ();

**Mouse Event**

There are eight types of mouse events:

Eight integer constants are defined to determine types:

 | MOUSE EVENT     | Generate                          |
 | --------------- |:--------------------------------:|
 | MOUSE_CLICKED	  | When user clicked the mouse       |

 | MOUSE_DRESSED	  | The user dragged the mouse        |

 | MOUSE_ENTERED	  | The mouse entered a component     |

 | MOUSE_EXITED	   | The mouse exited from a component |

 | MOUSE_MOVED	    | The mouse moved                   |

 | MOUSE_PRESSED	  | The mouse was pressed             |

 | 1MOUSE_RELEASED |	The mouse was released            |

 | MOUSE_WHEEL     |	The mouse wheel was moved.        | 

**Methods:**


int getX()

int getY()

Point getPoint() -> gives object that contain X, Y co-ordinates

int getClickCount()

boolean isPopupTrigger() -> tests if this events causes a pop-up menu to appear on this platform.

int getButton() -> returns a values that represents the button that caused the event.
