# midi2ip
This is very early pre-pre-pre-pre-alpha of a method to throw JACK MIDI reliably over an IP connection.  Not for any use at all yet.  Contributors encouraged!

To try it, [compile and] install the Mido library, and run these in separate xterms.  On this machine python3 didn't work for it, so:

python2 tcp2midi.py localhost:44440

python2 midi2tcp.py localhost:44440

then in your JACK patchbay, connect RtMidiIn-Client to your MIDI source, e.g., a USB MIDI interface attached to a keyboard controller, virtual MIDI keyboard, or anything else.  Send just one or two MIDI signals, and help figure out why so much data is passing through!
