# Exam questions

1. Describe dependency injection and inversion of control
    - Iverze kontroly je způsob řízení programu, kdy kontrolu nad vytvářením instancí tříd přebírá Spring, na základě dodané konfigureace
    - Při inicializaci programu jsou konkrétní instance tříd vytvořeny pomocí kontejneru frameworku Spring na základě připravené konfigurace.
    - Takto vytvořené instance jsou pak použity v místech programu, kde jsou deklarovány příslušné závislosti = Dependency Injection(DI)
    - Výhodou inverze kontroly je to, že v místě, kde jsem deklaroval závislost na třídě, nepotřebuji vytvořit konkrétní instanci a nemusím nastavovat všechny její parametry
    - Kontejner může podle konfigurace vytvořit jen jednu instanci třídy a tu použít na více místech programu
    - Kontejner lze konfigurovat pomocí anotací (v kódu) či externě pomocí XML
    - Dependency Injection je tedy návrhový vzor, který odstraňuje závislost z programovacího kódu, aby bylo možné aplikaci snadno spravovat a testovat. 
    - Dependency Injection dělá náš kód volně propojený

2. Describe Spring application container
    - Kontejner Springu je jádro frameworku Spring.
    - Jeho úkolem je vytváření objektů, jejich propojení, konfigurace a správa životního cyklu od vytvoření po odstranění
    - úkolem tříd reprezentující kontejner je: vytvoření kontejneru, konfigurace kontejneru, spojení komponent aplikace do jednoho celku
    - způsob vytvoření je: ručně pro standalone aplikace, nebo deklarací pro webové aplikace

3. Describe annotations
    - anotace slouží pro konfiguraci, stejně jako XML, anotace jsou flexibilnější než XML a lze je s ním i kombinovat, nebo s Java konfigurací
    - @autowired = anotace slouží k automatickému propojení vztahů mezi spolupracujícími beany 
                - Anotace @Autowired se defaultně chová jako „byType“ (Hledá bean příslušného typu a použije reference na něj)
   
    - @component
    
    - @configuration
    
    - @qualifier
    
    - @ComponentScan


4. What does bean represent in Spring

5. Describe difference between Singleton and Prototype bean scope

6. Describe bean lifecycle events