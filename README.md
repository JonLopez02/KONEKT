# KONEKT<br/>
Kaixo nire izena Jon López da eta hemen nire proiektuaren manuala eta zer behar dozun abiarazteko argituko dut.<br/>

INSTALAZIOA<br/>

Sql server<br/>
Sql Management Studio<br/>
.NET 6<br/>
Visual Studio<br/>
Auth0-an erregistratu<br/>

PROIEKTUAREN AZALPENA<br/>

Nire proiektuak bi klase ditu, user-ak eta mezuak. Biak konektatuta daude user-en id-a eta mezu bakoitzak mezuak bidaltzen duen id-a eta eragozten duen erabiltzailearen id-a. Bakoitzak bere funtzioak ditu.<br/>
Honen helburua da jendea librea edota errazagoa izatea bere arazoak edo osasun mentala gainontzeko.<br/>
Ez da lagunak egiteko helburuz printzipalean baina baliteke jendea hori ere egiteko asmoz sartu ditzakeela.<br/>
Proiektuaren parteak bananduta daude zer 25mb-ko artxibo baino handiagokoak ez du igotzen uzten. Barkatu eragozpenak.<br/>

GIDA<br/>

Hemen KONEKT zelan erabiltzeko gida bat da, horretaz aparte zer egin eta zer erramintak erabili behar diren argituko dira, ez bada klaru gereatzen gida manualean daukazu kapturekin eta gustiz.<br/>

ERREMINTAK<br/>
Visual Studio: https://visualstudio.microsoft.com/es/<br/>
Auth0: https://auth0.com/es<br/> 
Sql Server: https://www.microsoft.com/es-es/sql-server/sql-server-downloads<br/>
Sql Management Studio:<br/> 
https://docs.microsoft.com/es-es/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver15<br/> 
Blazor:<br/>
https://dotnet.microsoft.com/en-us/learn/aspnet/blazor-tutorial-vs/intro?adobe_mc_sdid=SDID%3D451F14B1893168FD-743A76BC93E4219F%7CMCORGID%3DEA76ADE95776D2EC7F000101%40AdobeOrg%7CTS%3D1652907425&adobe_mc_ref=https%3A%2F%2Fwww.google.com%2F<br/> 
Paqueteak: Entity Framework, auth0 token…<br/>

PROGRAMA<br/>
Programa hasieratzeko, blazor-a eta API-a batera hasieratu behar dituzu. Honela bi web zabalduko diraz. Bata blazor-a hau dela, index-a kargatzen du.<br/>
Beste aldetik, swagger-a, baina ez zaio kasurik egin behar. Klientea index-ean dago.<br/>

Index honetan 4 aukera daude, Admin, administratzaile moduan sartzen zarena eta Auth0 erabiltzen dena login-a egiteko. Login-a zer erabiltzaile moduan sartzeko asmoa baduzu erabiltzen da, ez ahaztu erregistratu behar zarela lehenengo. Erregistroa egiteko eta azkenik baina ez da hain inportantea, About orria.<br/>

REGISTER<br/>
Register aukeratzerakoa, erregistratzeko asmoa baduzu (ez bazara erregistratzen ezin duzu ezer egin dela eta). Pantaila hau agertuko zaizu:<br/>
Hemen zure erabiltzaile izena, pasahitza eta mail-a jarri behar duzu, honek balidatuta daude kondizio batzuetara. Mail-a “@gmail.com” karaktere antzerakoa eduki behar du. Pasahitza maiuskulako karaktere bat eta zenbaki bat eduki behar du. Idatzitakoan bakarrik “add” botoiari sakatu, eta index-era bueltatuko zara.<br/>

LOGIN<br/>

Oraingo honetan login egingo duzu kliente moduan:<br/>
Ikusiko duzunez oso erraza da, bakarrik zure erabiltzaile izena eta pasahitza jarri, eta logeatuko zara.<br/>

MEZUAK IKUSI<br/>

Login-a egiterakoan, ikusiko duzu Blazor nabegadorean gauza berri batzuk:<br/>
Mezuak idatzi, ikusi eta mezu zuzenak bidaltzeko orriak.<br/>
Ikusi ematerakoan honelako zerbait agertuko zaizu:<br/>
Ikusiko duzunez mezuen titulua ikusten da, baina titulu hauek link-ak dira, mezura bidaltzen dutenak. Mezuan barne idatzi ahal duzu bueltan pertsonari, edo, pertsona bere intentzio txarrez idazten ikusten baduzu, erreportatu egin ahal diozu. Admin-ak edo programa berak honetaz okupatuko dira. Kontuan hartu behin idatzita, pertsona horrek ezin izango dizu zuri bueltan idatzi zure erabiltzaile izena ez badauka.<br/> 

MEZUAK IDATZI<br/>

Ikustea bakarrik aspergarria da eta hemen zuk zure barnetxarrak esateko zaude. Beraz idazteko ahalmena duzu, mezu hau ausazko erabiltzaile bati helduko zaio. 
Titulua jarri eta gero idatzi zure sentimendu guztiak, ez daukazu limiterik. Amaitzerakoan bi aukera dituzu: Bidali horrela edo zure erabiltzaile izena eman (aurrerago azalduko du zertarako balio duen).<br/>

MEZU ZUZENAK IDATZI<br/>

Nire asmoa ez zen baina, mezua idazterakoan izena emateko ahalmena zenuen, hori da hemengo kasuan zuk besteen erabiltzaileen izena jakinduta, zuzenean mezua bidali ahal duzu. Honen helburua ez da “chat” bat egitea, baizik eta zuen artean lagundu eta zuen problemak errazago konpontzea al menos apur bat.<br/> 

ADMIN<br/>

Administratzaile bat bazara, Admin estekara joan behar zara login-a egiteko. Bertan zure erabiltzailea eta pasahitza sartu eta logeatuko zara (Auth0 zelan funtzionatzen duen jakiteko azkenengo orrietara joan).<br/>
Administratzailea, bere izenak esaten duen moduan administratu egiten du, dena. Mezu guztiak ikusi ahal dituzu:<br/>
Mezu honetan sartu ahal zara eta bertan irakurri, web-a pertsonala izan behar da, baina ziurtatu egin behar zara erabiltzaile guztiak onak izaten direla.<br/> 

Ikusterakoan mina egiten duen mezuak daudela edota inork irakurtzen edo erreportatzen dutela, zuk borratu ahal dituzu, “delete messages” estekan.<br/>
Hemen lista osoa ikusten da eta bere erabiltzaileen ID-ak. Ikusten duzunez ID bat eskatzen ari da. Jartzerakoan, mezua borratuko da erabiltzaile bietatik.<br/>

Admin bezala era mezu zuzenak bidali ahal dituzu erabiltzeileei arrazoi diferenteengatik, erreportatzeko abisu emanez edota nobedadeak emateko.<br/>
Azkenik erabiltzaile guztiak ikusi ahal dituzu:<br/>
Datu guztiak daude ikusgarriak direnak, eta inportanteena, erreporteak.<br/>

ERREMINTA ERABILTZEKO GIDA<br/>
AUTH0<br/>
Auht0 autorizazioak daukaten erabiltzaileetarako erabiltzen da, normalean administratzaileak izaten dira edota administratzaileen lankideak. Horretarako auth0-ren web orrira joan behar zara.<br/>
Hemen erregistratu behar zara gmail existente batekin. Egindakoan, “dashboard” agertuko zaizu.<br/>
Hemen gauza bi erabili ditut, aplikazioa eta erabiltzaileen esteka.<br/>
Aplikazioen estekan, bertan aplikazioaren izena, url-a etab… sartu beharko dira, gogoratu bertan tutorial bat dagoela galtzen bazara. Hemengo aplikazioko datuak ikustean ID-a eta authority-a kontuan hartu behar dira.<br/>
User managementan berriz, user-ak daukagu, autorizatuta daudenak, honek administratzaile moduan sartu ahal dira web orrira edota rol bat ematerakoan gauza ezberdinak lortu dezakete.<br/>
Programari begira, hauxe jarri beharko zenuke, appsettings-en (API) eta program.cs artxiboetan (Blazor).<br/>
