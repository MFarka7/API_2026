**Part 1**
 1) Přes API založte libovolného nového uživatele a automaticky zvalidujte, že:
    - zkontroluj, že reponse kód je 201,
    - emailVerified je nastaven na false
    - image je null (HINT: to.be.null)
 2) Přes DB potom takového uživatele vyhledejte. Výsledkem je tabulka, která bude mít níže uvedené sloupce:
    - Name,
    - Email,
    - CreatedAt,
    - Role

**Part 2**
 1) Pro vašeho uživatele založte nový účet a automaticky zvalidujte, že:
    - Reponse kód je 201,
    - isActive je nastaveno na true
    - email odpovídá emailu vámi založeného uživatele (HINT: v části 1 si nastavte tento email do proměnné kolekcí a zde použijte)
    - OPTIONAL: Pokud chcete účet si přejmenujte
 2) Přes DB potom vyhledejte všechny (tedy oba) účty vašeho uživatele. Výsledkem je tabulka, která bude mít níže uvedené sloupce:
    - Name – jméno vašeho uživatele,
    - Name – jména vašich účtů,
    - Number – čísla vašich účtů


**Pat 3**
 1) Pošlete dvě libovolné transakce z původního účtu na nově založený, a automaticky zvalidujte že:
    - Reponse kód je 201,
 2) Přes DB potom vyhledejte obě transakce tak, abychom ve výsledné tabulce měly:
    - Name – jméno vašeho uživatele,
    - Name – jméno účtu odkud transakce odešla (tj. jméno původního účtu),
    - Sent_from – číslo účtu odkud transakce odešla (HINT: potřebujete přejmenovat defaultní název sloupce)
    - Amount – velikost transakce, tedy kolik peněz jste poslaly (údaj z tabulky transactions),
    - Sent_to – číslo účtu na který byly obě transakce poslány tedy číslo účtu nového účtu (HINT: pro tento sloupec budete potřebovat select;-))


