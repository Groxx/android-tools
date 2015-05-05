# android-tools
Collection of things I've built while developing Android apps.

# Files include:
* ###[acp](acp)

  Runs whatever command you provide as the first argument, strips characters added by Mac's terminal (or whoever is to blame), and saves it to the file provided as the second argument.

  I primarily use this to extract databases from debuggable apps, without root permissions, using one of the examples in the help-text if you don't provide exactly two arguments.  But it works for any kind of binary output - e.g. if you capture a systrace with `acp 'atrace -z -a com.your.app' tmp.trace`, you can use it in `python systrace.py --from-file=tmp.trace`.  The possibilities are ENDLESS, use your power for awesome.
