# MAX78000
[MAX78000](https://www.maximintegrated.com/MAX78000) related things.

Modified demos that add GPIO pins and UART2 so they can communicate with another microcontroller like an Arduino.

- Cats-dogs demo: pin 2.3 indicates a cat, pin 2.4 is for dogs.

- Keyword spotting demo (KWS20): pin 2.3 toggles with 'On' and 'Off', pin 2.4 is high when confident.

Both demos output more verbose information on UART2 so it can be parsed by something else.

- Keyword spotting demo (KWS20), extended version as presented in [video](https://youtu.be/R-6A7q_bc6g): pin 2.3 toggles with 'On' and 'Off', pin 2.4 is high when confident (>95%), low if not. Port P1.6 pulses at 10 Hz for keywords 'One' (1 pulse) to 'Nine' and 'Zero' (ten pulses). 'Up' and 'Down' control the idle level of this pin (this simulates a rotary dial phone). UART2 (115200n81) transmits all detected keywords with confidence value in JSON format {"keyword":confidence}

