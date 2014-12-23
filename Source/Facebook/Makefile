MONOXBUILD=/Library/Frameworks/Mono.framework/Commands/xbuild

all: ios-unified ios-classic android

ios-unified: 
	$(MONOXBUILD) /t:Clean Facebook-MonoTouch.csproj
	$(MONOXBUILD) /p:Configuration=Release Facebook-MonoTouch.csproj

ios-classic: 
	$(MONOXBUILD) /t:Clean Facebook-MonoTouch-Classic.csproj
	$(MONOXBUILD) /p:Configuration=Release Facebook-MonoTouch-Classic.csproj

android:
	$(MONOXBUILD) /t:Clean Facebook-MonoDroid.csproj
	$(MONOXBUILD) /p:Configuration=Release Facebook-MonoDroid.csproj

clean:
	cd ../../ && rm -rf bin/