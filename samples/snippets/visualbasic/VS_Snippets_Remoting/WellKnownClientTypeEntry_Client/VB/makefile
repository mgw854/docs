all: WellKnownClientTypeEntry_Server.exe WellKnownClientTypeEntry_Client.exe

WellKnownClientTypeEntry_Server.exe: WellKnownClientTypeEntry_Server.vb WellKnownClientTypeEntry_Share.dll
	vbc WellKnownClientTypeEntry_Server.vb /r:WellKnownClientTypeEntry_Share.dll

WellKnownClientTypeEntry_Client.exe: WellKnownClientTypeEntry_Client.vb WellKnownClientTypeEntry_Share.dll
	vbc WellKnownClientTypeEntry_Client.vb /r:WellKnownClientTypeEntry_Share.dll

WellKnownClientTypeEntry_Share.dll: WellKnownClientTypeEntry_Share.vb
	vbc /t:library WellKnownClientTypeEntry_Share.vb
