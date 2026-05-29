# Hur du skapar en delbar länk för användartester
För att du ska slippa krångla med att deltagarna behöver ett konto i Claude, eller om du inte vill skicka iväg en HTML-fil till kund, kan du enkelt ladda ner en fristående HTML-fil av din prototyp från Claude och sedan lägga upp den på GitHub.

## Vad du behöver:  
* Claude Design
* Konto på GitHub

## Så här går du tillväga: 
### 1. Ladda ner standalone HTML från Claude Design
<ol type="a">
  <li>I din Claude-design, klicka på knappen <strong>Share</strong> uppe i höger och välj <strong>Export as standalone HTML</strong> i listan.</li>
  <li>Claude bistår nu med en nedladdningsknapp i chatten. Klicka på den för att ladda ner HTML-filen. </li>
  <li>Döp om den nedladdade HTML-filen till <code>index.html</code></li>
</ol>

### 2 Skapa nytt repository på GitHub
<ol type="a">
  <li>Beroende på var i GitHub du befinner dig klickar du antingen på knappen <strong>New</strong> bredvid rubriken <em>Top repositories</em>, eller går in på fliken <em>Repositories</em> och klickar på <strong>New</strong>.</li>
  <li><strong>Owner:</strong> Här väljer du dig själv (ditt användarnamn).</li>
  <li><strong>Repository name:</strong> För att din prototyp ska få en direktlänk måste namnet vara exakt <code>ditt-användarnamn.github.io</code> (byt ut "ditt-användarnamn" mot ditt faktiska namn på GitHub). Det fungerar alltså inte att döpa det till något annat.</li>
  <li><strong>Choose visibility:</strong> Välj <strong>Public</strong>. (Denna kan senare sättas till <em>Private</em> i inställningarna när du är helt klar med testerna).</li>
  <li>Klicka på <strong>Create repository</strong>. Övriga inställningar kan du lämna som de är.</li>
</ol>

### 3 Lägg till HTML-filen
<ol type="a">
  <li>Klicka på länken <strong>uploading an existing file</strong> i sektionen <em>Quick setup</em>.</li>
  <li>Dra och släpp din <code>index.html</code> i uppladdningsytan. Vill du testa flera prototyper kan du lägga filen i en mapp på din dator (t.ex. <code>min-fina-prototyp</code> – undvik mellanslag!) och dra in hela mappen.</li>
  <li>När filen har laddats upp klickar du på knappen <strong>Commit changes</strong>.</li>
  <li>Din prototyp finns nu live på <code>https://ditt-användarnamn.github.io</code> (alternativt <code>https://ditt-användarnamn.github.io/min-fina-prototyp/</code> om du la filen i en mapp).</li>
</ol>

## Extra: Hur uppdaterar jag min HTML-fil?
* **Ladda upp ny fil:** Gå till ditt repository, klicka på **Add file** och välj **Upload files**. Dra in din nya fil och repetera stegen 3b och 3c.
* **Redigera koden direkt:** Klicka på ditt befintliga `index.html` och välj penn-ikonen i verktygsfältet. Klistra in den nya koden över den gamla, klicka på **Commit changes...** och bekräfta i rutan som dyker upp.
* **Skapa en ny mapp direkt i GitHub:** Klicka på **Add file** och välj **Create new file**. För att skapa en mapp skriver du mappens namn följt av ett snedstreck (t.ex. `ny-mapp/`) och skriver därefter `index.html`. Klistra in din kod och spara, klicka på **Commit changes...** och bekräfta i rutan som dyker upp.
* **Ändra namn på mapp:** Klicka dig in hela vägen in till <code>index.html</code> och välj penn-ikonen för att redigera filen. Klicka på textfältet med filnamnet uppe till vänster om verktygslådan <code>index.html</code> och ställ textmarkören i början av filnamnet. Klicka sedan [<- backspace] på tangentbordet. Sedan skriver du bara in ditt nya mappnamn och avslutar med snedstreck `/`. Säkerställ att filnamnet fortfarande heter <code>index.html</code>. Alla ändringar du gör behöver sparas genom att klicka på **Commit changes...** och bekräfta i rutan som dyker upp.
