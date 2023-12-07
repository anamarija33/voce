
Resetiranje računala : `shutdown -r now`  
Gašenje računala : `shutdown -h now`  
Ažuriranje: `apt-get update` -> nadogradnja `apt-get upgrade`  




`ls [opcija] [datoteka/direktorij]` - izlistava sadržaj datoteka i direktorija  
	- `-l` - dugi format, prikazuje detaljnije informacije o datotekama i direktorijima  
	- `-a` - uključuje i skrivene datoteke i direktorije  
	- `-al`- dugi format i uključuje skrivene dat/dir  
	-`-ld /imedirektorija/ ` - prikazuje detalje samo za jedan direktorij   


`cd /direktorij/` - change directory - naredba za promjenu direktorija  
	- `cd /` - prebacuje u root direktorij  
	-`cd ~` ili `cd` - otvaranje home direktorija  
	- `cd ..` - vraćanje na direktorij iznad trenutnog  
	- `cd "ime direktorija"` - otvaranje direktorija koji ima razmak u imenu  



`pwd `- print working directory   


`touch datoteka`  - touch kreira (praznu) datoteku imena datoteka ako ne postoji   
	- može se kreirati više datoteka odjednom ` touch datoteka1 datoteka2 datoteka3`  


`cat datoteka` - čita sadržaj datoteke i ispisuje ga. Može kreirati, pregledavati ili spajati datoteke  
	- kreiranje/pregledavanje više datoteka odjednom: `cat datoteka1 datoteka2`  
	- `cat -n datoteka` - prikazuje sadržaj s numeriranim linijama  
	- `cat > datoteka` - kreiranje nove datoteke i dodavanje sadržaja  
	- `cat datoteka > datoteka_kopija` - kopira sadržaj datoteke u drugu datoteku  
	- `cat datoteka1 >> datoteka2` - dodaje sadržaj prve datoteke na kraj druge  
	- `cat "imedatoteke1" "imedatoteke2" "imedatoteke3" > "spojenedatoteke"`  - spaja više datoteka u jednu  
	- `cat *.txt` - ispisuje sadržaj svih tekstualnih datoteka u direktoriju  
	- `cat >> datoteka`- dodavanje sadržaja u postojeću datoteku  


`mkdir [opcije] [direktorij]` - kreira direktorij/mapu   
	- `mkdir direktorija`  
	- `mkdir -p dir1/dir2/dir3` - kreira parent direktorije   


`rmdir` - briše prazni direktorij     


`rm [opcije] [ime]` - briše datoteke/direktorije - direktorije ne briše po defaultu  
	- `rm datoteka`  
	- `rm -r direktorij` - rekurzivno briše sve iz mape i na kraju briše i mapu  


`cp [opcija] [izvorna dat/dir] [novoime]` - kopira datoteke/direktorije ili grupe dat/dir  
	- `cp dat dat2` - kopira sadržaj prve u drugu (ako postoji, obriše sadržaj i upiše novi bez upozorena), ako druga ne postoji, kreira je.   
	- `cp -R dir1 dir2`- rekurzivno kopira sadržaj u dir2, ako dir2 postoji dir1 postaje subdirektorij u dir2   


`mv [opcije] [izvornadat] [novadat]` - premješta ili preimenuje datoteke/direktorije  
	- `mv dir1 dir2` - preimenuje dir1 u dir2  
	- `mv dir1 /dir/dir3`- premješta datoteku dir1 u dir3  
	- `mv dir1 dir2 dir3 /home/dir/dir4/` - premještanje više datoteka/dir u direktorij  


`grep [options] pattern [files]` - pretražuje datoteku za dan uzorak teksta  
	- `grep 'Unix' datoteka.txt` - pretražuje i ispisuje sve linije teksta gdje je pronađen "Unix"  
	- `grep -i "Unix" datoteka.txt`- pretražuje linije teksta gdje se spominje unix, neovisno o veličini slova  
	- rekurzivno pretraživanje u direktoriju : `grep -R [string koji se pretražuje] [direktorij]`  


`find [where to start searching from] [expression determines what to find]`  
`[-options] [what to find]`  - pretražuje hijerarhiju mapa, može se koristiti za traženje datoteka i direktorija i obaviti neka operacija nad njima u isto vrijeme.  
	- `find /dir -name dat1.txt` - traži dat1.txt u dir direktoriju  
	- `find /dir -name *.txt` - traži sve tekstualne datoteke u dir hijerarhiji  


`tar [options] [archive-file] [file or directory to be archived]` - za kreiranje i raspakiravanje arhiva   
	


`nano ili vi ili jed` - za kreiranje i mjenjanje datoteke u tekstualnom editoru  
	- `nano` - otvara uređivač bez sadržaja  
	- `nano datoteka` - otvara uređivač sa sadržajem datoteke
	- > CTRL + O sprema datoteku CTRL + X izlazi iz programa  


`man` & `--help` - definicije naredbi  


`echo` - ispisuje poruku na standardni izlaz(monitor)  
	- `echo "neki text" >> test.txt`   


`zip [opcije] [datoteka.zip] [ime_dir]` / `unzip [zip dat]` arhiviranje / raspakiravanje arhiva  
	-`zip -r dat.zip dat/` - rekurzivno arhivira sve datoteke u direktoriju
 	- ` unzip dat.zip -d dat/` - otpakira arhivu u direktorij


`stat datoteka` - pogledaj statistiku datoteke  


`ln -s datoteka poveznica`- kreiranje poveznice (link)  
	-`unlink poveznica `-brisanje poveznice  
	-`rm poveznica`  

`wget datoteka*` - preuzmi datoteku s mreže  


`ping webstranica.hr` - provjeri mrežu prema serveru  


`history`- pregled povijest izvedenih naredbi  
	- `history n` - (n je broj) - ispiše zadnjih n naredbi  
	- `history -d n`- brisanje n linije iz povijesti  
	- `history -c`- brisanje povijesti  
	- `history tail`- prikazuje zadnjih 10 linija povijesti  


`alias`- pregledaj sva zamjenska imena naredbi  


`passwd` - promjena lozinke  


`top` - pregled stanja sustava  
	- `q` izlaz iz programa  


`more`- pregled sadržaja datoteke  


`head` - pregled početka datoteke  


`tail` - pregled kraja datoteke  


`date` - trenutno vrijeme  


`w` /`who` - podaci o spajanju korisnika  


`last` - popis spajanja korisnika  


`clear` - očisti sadržaj na zaslonu  

