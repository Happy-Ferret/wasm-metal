# WASM Metal

A bare metal physical implementation of WebAssembly. That's right, a WebAssembly CPU. Inspired in part by [this amazing talk](https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript).

## Development

### GUI Microarchitecture Simulator

```bash
git clone https://github.com/lastmjs/wasm-metal.git
cd wasm-metal
npm install
npm start
```

Go to [http://localhost:5000](http://localhost:5000) in your web browser.

### RTL Microarchitecture Simulator

Not implemented yet.

### Loading Microarchitecture Implementation to FPGA

Not implemented yet.

## Roadmap

- [ ] Understand the WebAssembly ISA
- [ ] Implement the mircoarchitecture in HTML/CSS/JavaScript
  * This will be a GUI simulator of the microarchitecture
  * This simulator will become the specification for the microarchitecture
  * It will allow us to quickly experiment with hardware configurations
  * It will allow us to iterate and learn how the microarchitecture should work
- [ ] Implement the microarchitecture as an RTL design in an HDL
- [ ] Simulate the RTL design
- [ ] Test the implementation on an FPGA
- [ ] Design the ASIC

## Why is this a good idea?

* [Maybe it's not](https://twitter.com/lastmjs/status/928682791511789568), but who cares
* The world is moving to WebAssembly
* Some of the biggest and potentially most world-changing projects are implementing their virtual machines as WebAssembly virtual machines (DFINITY, Ethereum)
* The bytecode is being designed as a compilation target for low-level languages first
* The bytecode is meant to execute at near-native speeds on a variety of underlying ISAs
* Java processors already offer potential benefits, even being compilation targets for a high-level language
* Cutting out the translation from WebAssembly to the underlying ISAs could provide efficiency benefits
* We could get rid of WebAssembly virtual machines entirely, and replace them with WebAssembly physical machines
* If [all SIM cards are Java processors](https://twitter.com/hedgeberg/status/935380806549286912), imagine what WebAssembly processors could do. I'm betting that WebAssembly is a better bytecode than Java bytecode for what Java bytecode is doing with microcontrollers, so WebAssembly could take over all spaces that Java processors currently have

## Prior art

* https://en.wikipedia.org/wiki/Jazelle
* https://stackoverflow.com/questions/1153076/does-android-castrate-the-arms-jazelle-technology
* https://en.wikipedia.org/wiki/Lisp_machine
* https://en.wikipedia.org/wiki/Java_processor
* https://en.wikipedia.org/wiki/High-level_language_computer_architecture
*
