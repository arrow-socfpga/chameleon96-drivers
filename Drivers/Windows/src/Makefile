all:	../Chameleon96_DRV.exe ../Chameleon96_D64.exe

../Chameleon96_DRV.exe:	Chameleon96_DRV.7z
	cat 7zSD.sfx config.txt Chameleon96_DRV.7z > ../Chameleon96_DRV.exe

../Chameleon96_D64.exe:	Chameleon96_D64.7z
	cat 7zSD.sfx config.txt Chameleon96_D64.7z > ../Chameleon96_D64.exe

Chameleon96_DRV.7z:
	cd files && 7za a ../$@ *
	cd dpinst && 7za a ../$@ dpinst.exe

Chameleon96_D64.7z:
	cd files && 7za a ../$@ *
	cd dpinst64 && 7za a ../$@ dpinst.exe

clean:
	rm Chameleon96_DRV.7z Chameleon96_D64.7z
