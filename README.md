
SS_Parser
==========

SS_Parser is a Parser to parser GSM  SS packet

Run a local web server, load ss.html file, decode SS packet

##example

###SS code

    0B 3B 1C 19 A1 17 02 01 00 02 01 0A 30 0F 04 01 29 83 01 10 84 07 80 20 51 80 20 27 F7 7F 01 00  

###ss parse:
````
SS BEGIN                :MT (0x8B)
Message type            :RELEASE COMPLETE (0x2A)
Information elements    :Facility (0x1C)
Faciltiy len            :11
        Component type  :Return Error (0xA3)
        Component len   :9
        Invoke ID tag   : (0x02)
        Invoke ID len   :1
        Invoke ID       :0
        Error Code tag  : (0x02)
        Error Code len  :1
        Error Code      :CallBarred (13)
````

