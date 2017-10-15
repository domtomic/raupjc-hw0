# Pitanje 1:
Nakon dodavanja class library-a kao referencu stvorila su se dva nova file-a: "ClassLibrary1.dll" i "ClassLibrary1.pdb", 
a nakon brisanja .dll file-a, program se ruši i javlja unhandled exception.
To se događa jer .dll sadrži PrintHelloWorld metodu koju glavni program referencira.
Potrebno je stoga imati .exe i .dll datoteku zajedno, tj. poslati ih skupa onome tko će koristiti program.

# Pitanje 2:
Program je koristio staru verziju class library asemblija jer novi nismo preveli, tj. spremili smo samo promjene u .cs file-u, 
a .dll je ostao isti.

# Pitanje 3:
Build proces se uspješno izvršio te je restoreao NuGet pakete, tj. u ovom slučaju vratio je NodaTime čiji se direktorij pojavio u packages direktoriju.