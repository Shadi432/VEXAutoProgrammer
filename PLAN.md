Pseudocode  for the VEX Auto Programmer

FILE *ProgramFile;
File = fopen("c:\\usd\\ProgramFile.txt", "a+");


if (SDCard is inserted) then
	if (SDCardHasFile(ProgramFile) then
		WAITFORBUTTONPERMISSIONTOBEGIN()
	else
		CREATENEWFILEONSDCARD()
		File = fopen("c:\\usd\\ProgramFile.txt", "w")
		WAITFORBUTTONPERMISSIONTOBEGIN()
	endif
else 
    CloseProgram()
endif

fClose(File)
