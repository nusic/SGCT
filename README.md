SGCT
====

Se https://c-student.itn.liu.se/wiki/ för mer information om SGCT.

För att se tillgängliga kommandon se make help

	// lista kommandon
	$ make help 

SGCT fungerar för windows (mingw 4.7.0), linux och mac.

    // Kompilera projektet
    $ make
	
	// kompilera med gtest (fungerar ej på windows än)
	$ make TEST=1
	
	// kompilera med ljud kräver viss handpåläggning med installation av openal, se c-student för mer info.
	$ make SOUND=1
	
	// ta bort objektfilerna
	$ make clean
	
För att köra programmet finns det en körfil som heter sgct_sim.sh. Windows kräver att msys finns med sh i path.

	// köra simulator (linux och mac)
	$ ./sgct_sim.sh
	
	// windows
	$ sh sgct_sim.sh
	
	// för att starta VR-simulator
	$ ./sgct_sim.sh VR
	
Det finns installationsscript för att snabbare komma igång biblioteken för ljud med ubuntu, mac och windows. (alla tre kräver administratörsrättigheter)

	// ubuntu
	$ make install-ubuntu
	
	// mac
	$ make install-macosx
	
	// windows
	$ make install-windows