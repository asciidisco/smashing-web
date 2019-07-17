# smashing-web

This repository contains a few examples on how to connect with USB & Bluetooth devices via the
WebUSB & WebBluetooth interfaces.

## TOC Examples

* `webusb` - WebUSB examples
  - `01-connect-device` - Connect to a device via WebUSB & display its meta data
  - `02-print-text` - Connect to POS compatible printer & print text
  - `03-canvas-to-print` - Connect to POS compatible printer & print the contents of a `<canvas>` element
  - `04-hid-devices` - Use a USB barcode scanner to scan ISBN numbers from books barcodes & retrieve some meta data from an online service

* `webbluetooth` - WebBluetooth examples
  - `01-connect-device` - Connect to a device via Bluetooth & display its meta data
  - `02-heartrate` - Connect a heart rate monitor device & display the heart rate
  - `03-lightbulb` - Connect to compatible Bluetooth lightbulb & steer it

## Used devices

* [Heart Rate Monitor](https://www.amazon.de/BerryKing-Heartbeat-Bluetooth-RUNTASTIC-Herzfrequenzmesser/dp/B0182GISA2/ref=sr_1_3?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=bluetooth+heart+rate+monitor&qid=1563360506&s=gateway&sr=8-3)
* [Bluetooth Lightbulb](https://www.ebay.de/itm/4x-XAVAX-Bluetooth-LED-Lampe-E27-7W-2700K-530lm-AGL-RGB-A-Gluehbirne-Gluehlampe-/254174270030)
* [POS Printer](https://www.amazon.de/FENGT-Thermodrucker-Portable-Bluetooth-Kompatibel/dp/B07HNGS125/ref=sr_1_2?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=58hu&qid=1563360489&s=gateway&sr=8-2)
* [Barcode scanner](https://www.amazon.de/CSL-Barcodescanner-Handscanner-Installation-ergonomisches/dp/B07BGW356L/ref=sr_1_4?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&keywords=usb+barcode+scanner&qid=1563360532&s=gateway&sr=8-4)

## Further resources

### Web Bluetooth

* [WebBluetooth API - Draft](https://webbluetoothcg.github.io/web-bluetooth/)
* [Interacting with Bluetooth Devices on the web](https://developers.google.com/web/updates/2015/07/interact-with-ble-devices-on-the-web)
* [Web Bluetooth API @MDN](https://developer.mozilla.org/en-US/docs/Web/API/Web_Bluetooth_API)

### Web USB

* [WebUSB API - Draft](https://wicg.github.io/webusb/)
* [Control an Arduino with WebUSB](https://harbaum.github.io/ftduino/webusb/en/)
* [WebADB - Connect Android devices via WebUSB](https://github.com/webadb/webadb.js)
* [Building a device for WebUSB](https://developers.google.com/web/fundamentals/native-hardware/build-for-webusb/)

### POS Printers

If you'd like to dig further into programming POS printers, have a look at [ESC/POS Mode Command Specifications](http://www.starmicronics.com/support/mannualfolder/escpos_cm_en.pdf) which describe all the commands from the POS spec that can be send to compatible printers in order to make some art™

## Running the examples

Any webserver will do, if you have Node.js installed, just run

```bash
npx http-server -p ${PORT}
```

and you're good to go.