<header>

<!--
  <<< Author notes: Course header >>>
  Include a 1280×640 image, course title in sentence case, and a concise description in emphasis.
  In your repository settings: enable template repository, add your 1280×640 social image, auto delete head branches.
  Add your open source license, GitHub uses MIT license.
-->

# Testimine Actionsiga

_Loo töövoogusid, mis võimaldavad kasutada pidevat integratsiooni (CI) sinu projektides._

</header>

<!--
  <<< Author notes: Course start >>>
  Include start button, a note about Actions minutes,
  and tell the learner why they should take the course.
-->

## Tere tulemast

[Pidev integratsioon](https://en.wikipedia.org/wiki/Continuous_integration) aitab sul järgida oma meeskonna kvaliteedistandardeid, käivitades teste ja raporteerides tulemusi GitHubis. CI tööriistad käivitavad ehitusi ja teste, mida käivitavad commit'id. Tulemused postitatakse tagasi GitHubi pull request'i. Eesmärk on vähem probleeme `main` harus ja kiirem tagasiside töötamise ajal.

- **Kellele see on**: Arendajatele, DevOps inseneridele, uutele GitHubi kasutajatele, õpilastele, meeskondadele.
- **Mida õpid**: Mis on pidev integratsioon, kuidas kasutada GitHub Actionsi CI jaoks, kuidas luua töövoog, mis käivitab teste ja toodab testiraporteid.
- **Mida ehitad**: Kasutame [remark-lint](https://github.com/remarkjs/remark-lint)'i Markdown-failide järjepidevuse kontrollimiseks.
- **Eeltingimused**: Eeldame, et oled esmalt läbinud [Tere GitHub Actions](https://github.com/skills/hello-github-actions) kursuse.
- **Kestus**: Selle kursuse saab lõpetada vähem kui kahe tunniga.

Sellel kursusel sa:

1. Lisad testi töövoo
2. Parandad testi
3. Laadid üles testiraporti
4. Lisad haru kaitsed
5. Ühendad oma pull request'i

### Kuidas seda kursust alustada

<!-- For start course, run in JavaScript:
'https://github.com/new?' + new URLSearchParams({
  template_owner: 'HKHK-Skills',
  template_name: 'test-with-actions',
  owner: '@me',
  name: 'skills-test-with-actions',
  description: 'Minu kursuse repo',
  visibility: 'public',
}).toString()
-->

[![start-course](https://user-images.githubusercontent.com/1221423/235727646-4a590299-ffe5-480d-8cd5-8194ea184546.svg)](https://github.com/new?template_owner=HKHK-Skills&template_name=test-with-actions&owner=%40me&name=skills-test-with-actions&description=Minu+kursuse+repo&visibility=public)

1. Tee paremklikk nupul **Start course** ja ava link uuel vahekaardil.
2. Uuel vahekaardil täituvad enamik välju automaatselt.
   - Omanikuks (owner) vali **oma organisatsioon** (mitte isiklik konto!).
   - Soovitame luua avaliku (public) repositooriumi, kuna privaatsed repod [kasutavad Actions minuteid](https://docs.github.com/billing/managing-billing-for-github-actions/about-billing-for-github-actions).
   - Keri alla ja kliki vormi allosas nuppu **Create repository**.
3. Pärast uue repositooriumi loomist oota umbes 20 sekundit, seejärel värskenda lehte. Järgi samm-sammult juhiseid uue repositooriumi README-s.

<footer>

<!--
  <<< Author notes: Footer >>>
  Add a link to get support, GitHub status page, code of conduct, license link.
-->

---

Abi saamiseks: [HKHK-Skills Discussions](https://github.com/orgs/HKHK-Skills/discussions)

&copy; 2023 GitHub &bull; [Käitumisjuhend](https://www.contributor-covenant.org/version/2/1/code_of_conduct/code_of_conduct.md) &bull; [MIT litsents](https://gh.io/mit)

</footer>
