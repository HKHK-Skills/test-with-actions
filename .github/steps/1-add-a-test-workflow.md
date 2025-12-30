<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
-->

## Samm 1: Lisa testi töövoog

_Tere tulemast kursusele "GitHub Actions: Pidev integratsioon"! :wave:_

**Mis on _pidev integratsioon_?**: [Pidev integratsioon](https://en.wikipedia.org/wiki/Continuous_integration) aitab sul järgida oma meeskonna kvaliteedistandardeid, käivitades teste ja raporteerides tulemusi GitHubis. CI tööriistad käivitavad ehitusi ja teste, mida käivitavad commit'id. Kvaliteeditulemused postitatakse tagasi GitHubi pull request'i. Eesmärk on vähem probleeme `main` harus ja kiirem tagasiside töötamise ajal.

![Illustratsioon vasaku ja parema poolega. Vasakul: illustratsioon kuidas GitHub Actionsi terminid on kapseldatud. Kõrgeimal tasemel: töövood ja sündmuse käivitajad. Töövoogude sees: tööd ja ehituskeskkonna definitsioon. Tööde sees: sammud. Sammude sees: kutse action'ile. Paremal: hinnatud järjestus: töövoog, töö, samm, action.](https://user-images.githubusercontent.com/6351798/88589835-f5ce0900-d016-11ea-8c8a-0e7d7907c713.png)

- **Töövoog**: Töövoog on automatiseerimisühik algusest lõpuni, kaasa arvatud mis käivitab automatiseerimise, millist keskkonda või teisi aspekte tuleks automatiseerimise ajal arvestada ja mis peaks käivitaja tulemusena juhtuma.
- **Töö**: Töö on töövoo sektsioon ja koosneb ühest või rohkemast sammust. Selles meie töövoo sektsioonis defineerib mall sammud, mis moodustavad `build` töö.
- **Samm**: Samm esindab ühte automatiseerimise _efekti_. Samm võib olla defineeritud GitHub Actionina või teise ühikuna, nagu konsooli printimine.
- **Action**: Action on automatiseerimistükk, mis on kirjutatud töövoogudega ühilduvalt. Action'eid võib kirjutada GitHub, avatud lähtekoodiga kogukond või sina ise!

Lisainfo saamiseks vaata [Workflow syntax for GitHub Actions](https://docs.github.com/actions/using-workflows/workflow-syntax-for-github-actions) GitHub Docs'is.

Esmalt lisame töövoo meie Markdown-failide lint'imiseks (puhastamiseks, nagu lint-rull) selles repositooriumis.

### :keyboard: Tegevus: Lisa testi töövoog

1. Ava uus brauseri vahekaart ja tööta järgmiste sammude kallal selles vahekaardis, lugedes juhiseid sellel vahekaardil.
1. Mine **Actions** vahekaardile.
1. Kliki **New workflow**.
1. Otsi "Simple workflow" ja kliki **Configure**.
1. Nimeta oma töövoog `ci.yml`.
1. Uuenda töövoogu, kustutades kaks viimast sammu.
1. Lisa järgmine samm oma töövoo lõppu:
   ```yml
   - name: Käivita markdown lint
     run: |
       npm install remark-cli remark-preset-lint-consistent
       npx remark . --use remark-preset-lint-consistent --frail
   ```
   > Isegi kui kood on `ci.yml` failis korralikult taandatud, näed GitHub Actionsis ehitusviga. Parandame selle järgmises sammus.
1. Kliki **Commit changes...** ja vali luua uus haru nimega `ci`.
1. Kliki **Propose changes**.
1. Kliki **Create pull request**.
1. Oota umbes 20 sekundit ja seejärel värskenda seda lehte (seda, kus sa juhiseid loed). [GitHub Actions](https://docs.github.com/actions) uuendab automaatselt järgmise sammu juurde.
