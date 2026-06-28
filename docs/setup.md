---
sidebar_position: 2
---

# Garść podstawowych informacji

## Wymagania

Przykłady były przetestowane w _node_ `v18.15.0`.
Do napisania przykładów wykorzystano _Arduino Uno_. W przypadku innych urządzeń piny i setup może się różnić.
Do sprawdzenia pod jakim portem podpięty jest sprzęt użyj `npx @serialport/list`.

Przykładowo:

```sh
❯ npx @serialport/list
/dev/tty.wlan-debug
/dev/tty.Bluetooth-Incoming-Port
/dev/tty.usbmodem1301  Arduino (www.arduino.cc)
```

Czasem przykłady będą wczytywać port ze zmiennych środowiskowych przy pomocy paczki `dotenv`. Nic nie stoi na przeszkodzie, by przekazać wartość w ten sposób:

```js
const board = new Five.Board({
  port: '/dev/tty.usbmodem1301',
});
```

## Przygotowanie Arduino Uno + Johnny Five

Przeczytaj: <https://johnny-five.io/platform-support/#arduino-uno> z uwzględnieniem <https://github.com/rwaldron/johnny-five/wiki/Getting-Started#trouble-shooting>
