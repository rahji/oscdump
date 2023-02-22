# OSC Dumper

This is a simple command-line tool that serves as an OSC server, dumping everything it receives from an OSC client to the screen (STDOUT). Good for testing.

It comes almost entirely from one of the examples in the [go-osc package](https://github.com/hypebeast/go-osc). I made a few changes and created this repository to make it easy to download and use for anyone (not just Go programmers).

## Installation

1. Download the appropriate archive file from the [Releases](https://github.com/rahji/oscdump/releases/latest) page.
2. Place the `oscdump` executable somewhere
3. Open a terminal window. (On MacOS, use the Terminal app. On Windows, you might need to [download Windows Terminal](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701?hl=en-us&gl=us&rtc=1) from Microsoft.)
4. Change to the folder where you placed `oscdump`
5. Execute the command using the instructions below

## Usage

### On Your Computer

Open a terminal window and run the command like so: 

```bash
./oscdump 192.168.4.20 8000
```

(Use your own IP address, of course).

### On Your Phone or Another Computer

1. Start an OSC client application ([TouchOSC mk1](https://hexler.net/touchosc), [MultiSense OSC](https://play.google.com/store/apps/details?id=edu.polytechnique.multisense.release&gl=US), etc.)
2. Verify that the app's settings for the server IP address and port match what you typed above.

You should start seeing OSC messages printed on the screen from the client.

### To Quit

Press `Ctrl-C` to quit the program.

## License

MIT: Same as [the go-osc license](https://github.com/hypebeast/go-osc/blob/master/LICENSE).
