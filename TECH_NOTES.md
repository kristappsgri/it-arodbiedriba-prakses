Tehniskais apraksts - kā tas viss strādā

Kādas tehnoloģijas tiek izmantotas:

- HTML - lapas struktūrai
- CSS - izskatam un noformējumam  
- JavaScript - lai pieslēgtos Supabase un parādītu datus
- Supabase - datu bāze, kur glabājas biedru saraksts
- GitHub - projekta glabāšanai un versiju kontrolei

Konfigurācijas faili:

Šim projektam nav atsevišķa .env faila. Supabase atslēgas (URL un anon key) ir ieliktas tieši index.html failā, jo tas ir mācību projekts.

ATGĀDINĀJUMS SEV: Īstās atslēgas nedrīkst likt repozitorijā publiski! Reālos projektos atslēgas glabā .env failā, kas ir pievienots .gitignore.

Kurā failā atrodas kods, kas pieslēdzas Supabase un nolasa datus?

Fails: index.html

Īss komentārs: 
- Rinda "const mySupabase = window.supabase.createClient(...)" izveido savienojumu ar Supabase
- Funkcija "loadMembers()" nolasa datus no "members" tabulas un parāda tos lapā
- Dati tiek attēloti kartīšu veidā ar biedra vārdu un statusu
