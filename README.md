# AscomSwitchDriver
Simple ascom driver for a cheap relay switch board,
configured for 2 channel relay board.
Requires modifying .iss script, which is then compiled and ran in inno to generate the installer exe


## Other notes:
Works with boards that take status query byte "0xFF", and response with format string of "CH1:OFF \r\nCH2:OFF \r\n" etc.
Open 1st channel: A0 01 01 A2
Close 1st channel : A0 01 00 A1

Open 2nd channel : A0 02 01 A3
Close 2nd channel : A0 02 00 A2
