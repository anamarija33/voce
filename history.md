    1  ls  
    2  cd Voce  
    3  ls  
    4  cd Jabuke  
    5  mkdir grannySmith pinkLady  
    6  touch grannySmith/Info.txt  
    7  touch pinkLady/Info.txt  
    8  cd ..  
   10  tree Voce  
   28  mkdir Limun Naranca  
   29  ls  
   30  touch Limun/Info.txt Naranca/Info.txt  
   31  tree  
   33  cd Documents/vjezba/Voce/  
   34  ls  
   35  cd Jabuke/  
   36  cd grannySmith/  
   37  ls  
   38  nano Info.txt   
   39  echo "I ukusne" > Info.txt  
   40  nano Info.txt   
   41  echo "Granny Smith jabuke su zelene i kisele" >> Info.txt  
   42  nano Info.txt   
   49  ls -l Voce/Jabuke/grannySmith/ >> listaDatoteka.txt  
   50  nano listaDatoteka.txt   
   51  nano Voce/Jabuke/pinkLady/Info.txt   
   52  nano Voce/Citrusi/Naranca/Info.txt   
   57  grep -r "zelene" Voce  
   65  sort /Voce/Jabuke/grannySmith/Info.txt >> sortiranoVoce.txt  
   66  cd Voce/Jabuke/grannySmith/  
   67  sort Info.txt >> sortiranoVoce.txt  
   68  nano sortiranoVoce.txt   
   69  cd ../../..  
   94  ls  
   96  zip Voce.zip -r Voce/  
   97  unzip Voce.zip -d RaspakiranoVoce  
   98  ls  
   99  cd RaspakiranoVoce/  
  100  tree  
  101  cd ..  
  102  wget https://pandoc.org/MANUAL.html  
  103  cat MANUAL.html   
  104  cd Voce/Jabuke/grannySmith/  
  105  ls  
  106  nano Info.txt   
  107  diff Info.txt sortiranoVoce.txt   
  108  cd ../../../..  
  109  cd vjezba/  
  110  history  
  111  man touch   
  112  history 20 >> povijestNaredbi.txt  
  113  ls  
  114  nano povijestNaredbi.txt   
  115  man ls  >> manualLs.txt  
  119  cat manualLs.txt   
  120  head manualLs.txt   
  121  tail manualLs.txt   
  124  touch voceDokumentacija.md  
  125  ls  
  126  nano voceDokumentacija.md   
  127  cat voceDokumentacija.md >> MarkdownPrikaz.txt   
  128  cat MarkdownPrikaz.txt    
  129  ls    
  130  pandoc -s -o voceDokumentacija.html voceDokumentacija.md    
  131  ls  
  132  ls >> potvrdaKonverzije.txt   
  133  ls    
  134  cat potvrdaKonverzije.txt      
  135  open ./voceDokumentacija.html   
  137  history >> history.md  
