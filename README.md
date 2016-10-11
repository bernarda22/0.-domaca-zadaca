# 0.-domaca-zadaca
osobni podaci

# JMBAG
0036471071

# Pitanje 1.
Primjećujem da se kod bin/debug foldera konzolne aplikacije, nakon što je dodan class library, pojavio pripadni Program Debug Database (.pdb) te asemblij s ekstenzijom .dll.
Nakon što maknem asemblij .dll iz foldera konzolne aplikacije .exe se ne može izvršiti jer CLR ne može naći međukod, odnosno potreban asemblij. ClassLibrary1.dll asemblij se ne nalazi na GAC-u, s kojim CLR komunicira, kao u prethodnom slučaju te se za izvršavanje programa on mora nalaziti u folderu kako bi CLR uspješno izvršio program.
Poslat ću asemblije .exe i .dll

# Pitanje 2.
Ako ne prevedemo izmjenjeni kod konzolna aplikacija koristi staru verziju class library asemblija. Zato što novi (izmjenjeni) kod nismo preveli u .dll i virtualna mašina (CLR) ima pristup starom asembliju s neizmjenjenim MSIL-om.

# Pitanje 3.
Ispisalo se: "Pero: Hello World"

# Pitanje 4.
U bin/debug folderu konzolne aplikacije pojavio se pripadni asemblij PeroClassLibrary.dll

# Pitanje 5.
Nakon što obrišem originalni .dll na disku aplikacija i dalje radi. Path za asemblij je ostao također isti iako je orginalni .dll obrisan. Vjerojatno je program napravio kopiju unutar vlastitog projekta.

# Pitanje 6.
Tijekom buildanja program je poslao poruku da je NuGet downloadao paket koji nedostaje. U packages direktoriju pojavio se NodaTime direktorij.
