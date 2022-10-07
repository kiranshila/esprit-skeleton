# An Example Project for Esprit

Checkout [Esprit](https://github.com/mfikes/esprit) for more info.

Many aliases are provided to automate the majority of the "embedded workflow". These can easily be incorporated into a Makefile if need be.

To erase the ESP32:
``` shell
clj -M:erase
```

To bootstrap Espruino onto the ESP32:
``` shell
clj -M:bootstrap
```

To compile the CLJS build:
(You will probably need to change the WiFi settings in `resources/secrets.edn`)
``` bash
clj -M:build
```

To create the ROM:
``` bash
clj -M:rom
```

To flash the ROM to the ESP32:
``` shell
clj -M:flash
```

To connect to the REPL:
(You will probably need to change the endpoint address in `resources/repl-opts.edn`)
``` shell
clj -M:repl
```
