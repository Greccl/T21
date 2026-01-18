# T21
A specification for building terminal emulators for the 21st century.



## Why?

Terminal emulators are a powerful, useful, and widely used tool. But current implementations must deal with several
protocols that exist in parallel, supporting features designed for hardware that no longer exists.

The goal of T21 is to eliminate mandatory support for features that were designed for older hardware and provide
support for the way terminal emulators are used today. For example, key combinations like ***ctrl+m*** and ***ctrl+h*** are
translated to other events and keystrokes are not reported exactly as they occur, reducing the number of keyboard
shortcuts that can be used, so T21 proposes a mechanism to inform the application using a terminal about rich
keyboard events, allowing a mode where keystrokes are reported not only as printable characters but also as
physical events.

T21's objectives are:
- Eliminate the need to use terminfo and termcap databases.
- Remove support for features that are not relevant to current terminals.
- Unify features that have several different specifications.
- Take advantage of the advanced graphics features of current operating systems.
- Provide advanced access to input methods such as keyboard and mouse.
- Simplify the construction of text-based graphical interfaces.



# License

This specification is licensed under the Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0).  
See the LICENSE file for details.

This license applies to the specification text, not to implementations.

## Copyright

© 2026 Leandro Damian Grecco
