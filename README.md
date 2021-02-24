# MAX78000
[MAX78000](https://www.maximintegrated.com/MAX78000) related things.

Modified demos that add GPIO pins and UART2 so they can communicate with another microcontroller like an Arduino.

- Cats-dogs demo: pin 2.3 indicates a cat, pin 2.4 is for dogs.

- Keyword spotting demo (KWS20): pin 2.3 toggles with 'On' and 'Off', pin 2.4 is high when confident.

Both demos output more verbose information on UART2 so it can be parsed by something else.
