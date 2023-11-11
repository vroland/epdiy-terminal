Epdiy Terminal
===============

Implements a serial terminal on an [epdiy](https://github.com/vroland/epdiy) ePaper controller.

Quickstart:

1. Build and flush: `idf.py build && idf.py flash -b 921600`
2. Write to the TTY, e.g. `script -f /dev/ttyUSB0`

Known Issues:

- With ESP-IDF 4.0, there is seems to be an issue with the UART 
  leading to missing / delayed data in some cases.
  Seems to be gone in 4.1. Enabling UART ISR in IRAM might help.


## Licese
- [st](https://st.suckless.org/) is licensed under MIT/X Consortium License (see [`main/LICENSE`](./main/LICENSE)).
