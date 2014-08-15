Starfall Chips from glebqip
=============

Uses Mujyuoon starfall:
  https://github.com/Mijyuoon/starfall

Chips have a unique name:chiptype_*_tooltype(_unfinished)
Chiptypes:
  sub - Metrostroi chips(link:http://steamcommunity.com/sharedfiles/filedetails/?id=261801217)
  stargate - CAP chips(link:http://facepunch.com/showthread.php?t=1250181)
  Warning: stargate chips may not work, because they are be created for older version of CAP
Tooltypes:
  proc - Starfall Processor
  remote - Starfall Remote
  screen - Starfall Screen

lib - special libs(big thanks to Mijyuoon)

dialing_computer - Dialing computer screen from first 2 seasons of stargate series
  Inputs:
    Stargare - stargate wirelink input, connect to stargate
    Keyboard - keyboard input, connect to keyboard Memory output
    AddrIn   - Address book input, connect to Address book AddrOut output
  Work:
    A-Z keys to enter address.
    Enter to start dialing.
    Backspace to remove a inputed symbol or close a gate.
    "\" to open\close IRIS.
    "=" to show gate open time.
    Numpad
      1 - to standart dialing mode
      2 - to fast dialing mode
      3 - to nox dialing mode
address_book - Address book screen from first 2 seasons of stargate series
  Inputs:
    Stargare - stargate wirelink input, connect to stargate
  Outputs:
    AddrOut  - Address book chosed address out.
  Work:
    Up and Down arrow to scrool addresses.
    Left and Right arrow to choose address.
    Enter to send address to Dialing computer(AddrOut), or start dialing if pressed again.
idc_screen - IDC screen from first 2 seasons of stargate series
  (unfinished)

vityaz - Vityaz screen(http://ic.pics.livejournal.com/drugoi/484155/2426194/2426194_original.jpg)
  Inputs:
    Train - Train input, connect to 81-717 train
  Outputs:
    Test  - debug output
  (unfinished)

autodrive(proc) - 81-717 autodrive system(uses autodrive_informator)
  Inputs:
    Train     - first wagon input, connect to first wagon
    TrainLast - last wagon input, connect to last wagon
  Outputs:
    Test,Test1 - debug outputs
  Work:
    First, choose a route on special panel(First and last station)
    Start button - start a autodrive system(train starts move)
    BCCD - Button Concorde Closed Doors,uses when doors need be closed(ring start), stops a ring
    Or press a space(Attention Pedal) to stop ring(need when not to closing the doors)

autodrive(screen)
  Inputs:
    Train - Train input, connect to 81-717 train(or Ezh3)
  Shows a some train info.

informator
  Inputs:
    Train - Train input, connect to 81-717 train
  Work:
    Informator "+" or "-" - choose a setting or scrool announce
    First, setup it:
      1 - Press Menu to start setting
      2 - Choose start station, press Menu;
      3 - Choose last station, press Menu;
      4 - Choose path of move, "+" for I path, "-" for II path;
      5 - Choose playing style(Moscow, St. Petersburg, Kiev), press Menu;
      6 - Confim settings with Menu, or press "+"/"-" to reset;
    I programm (tumbler Programms down) - play announce
    II programm (tumbler Programms up)  - play special announce
    Menu when configured - go to Confim stage(5)

shunt_panel
  Work:
    First, take a tablet and press E on chip.
    Then, press E to connect to train(works only with 81-717(not 714))
    Press ALT+Left Mouse to enable keyboard
    Press ALT+Right to zoom in(out)
    Tabs
      1:Shunt panel
        QWE - first tumblers row
        RTY - second tumblers row
        ASD - first buttons row
        ZXC - second buttons row
        FG  - revers backward\forward
      2:Breakers
        (unfinished)
      3:Value 013(334)(Is selected in the code, 89 and 401 line(Type variable). 1 for 334, 2 for 013)
        ";" and "'" - incerace(decerace) position
        L           - driver value disconnect value
      4:ARS Panel
        (unfinished)
      5:Lamps
        (obsolete, will be deleted)
