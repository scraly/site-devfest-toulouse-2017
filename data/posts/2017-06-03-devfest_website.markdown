Comme tous les évènements tech, le DevFest nécessite d'avoir un site web de bonne qualité pour pouvoir vous communiquer des informations, les avancées sur l'évènement, les speakers, le programme... en fait tout ce qui est important est sur notre site !

Dans [l'équipe](https://devfesttoulouse.fr/team/), nous sommes tous des développeurs (peut être certains moins que d'autres... 😀), nous avons donc voulu pouvoir mettre à jour le site, sans fatigue, sans stress et de manière collaborative et totalement automatisée (feignant comme un dev qu'il dit l'autre).

<img src="/images/posts/2017-06-03-devfest_website/website.png" alt="website" width="500" />

Nous sommes partis de l'excellent [projet Hoverboard](https://github.com/gdg-x/hoverboard) créé et maintenu par l'équipe du [GDG Lviv | DevFest Ukraine](https://devfest.gdg.org.ua/team/) que nous remercions grandement au passage.

Comme tout bon projet, il est totallement OpenSource (licence MIT) et tout le monde peux l'utiliser, le modifier et contribuer, ce que nous n'avons pas hésité à faire pour corriger des bugs, faciliter le développement ou même améliorer des fonctionnalités !  

<img src="/images/posts/2017-06-03-devfest_website/gdg-x-hoverboard.png" alt="hoverboard" width="500" />


# Et en vrai, c'est fait avec quoi ce site ?

Je vais en réjouir certains, peut être décevoir d'autres qui souhaiteraient voir leur technologie préférée utilisée pour ce projet... Mais dans le fond, on s'en fout un peu, du moment que cela fonctionne et que que cela est simple à prendre en main, c'est l'essentiel !

Dans notre cas, la stack technique utilise Polymer pour la partie front et du Firebase pour la partie "backend". Nous sommes vraiment dans la mouvance "Server-less" (ou dans notre cas, le server, c'est Google 😉)

<img src="/images/posts/2017-06-03-devfest_website/firebaseandpolymer.png" alt="polymer and firebase" />

Ces technologies nous permettent de transformer notre simple site web en Progressive Web Application (PWA). Vous pouvez consulter l'intégralité du site hors-ligne à partir du moment où vous l'avez visité une fois, pratique lors de la conf si l'on a pas beaucoup de réseau !

<img src="/images/posts/2017-06-03-devfest_website/pwa.png" alt="pwa" width="300" />

 
# Et qui se charge des mises à jours du site ?

Nous travaillons en équipe, les mises à jours se font donc en équipe. Il vous suffit de regarder notre flux de commit sur le [projet Github du site](https://github.com/GDGToulouse/site-devfest-toulouse-2017) et vous verrez que tout le monde met la main à la pate.

Nous fonctionnons par Pull-Request, chaque personne de l'équipe, quand il souhaite faire une modif sur le site doit soumettre une PR qui sera analysée par quelqu'un d'autre qui acceptera ou refusera la modification.

<img src="/images/posts/2017-06-03-devfest_website/commit-flow.png" alt="pwa" width="600" />

Cet article ne fera pas exception et sera donc intégré à une PR comme toutes modifications du site...
 

# Et qui se tape tous les déploiements ?

Bien que je vous ai dit plus tôt que c'était un travail d'équipe, sur le point du déploiement, tout est à la charge d'une seule personne afin d'assurer la continuité du déploiement... et ce taff, c'est Travis qui s'en charge ! 
 
L'avantage avec Travis, c'est qu'il s'intègre de la meilleur des manières avec Github et Firebase. Résultat, chaque commit sur master entraîne un déploiement sur Firebase en automatique. 0 effort pour l'équipe.

<img src="/images/posts/2017-06-03-devfest_website/git-github-travis.png" alt="pwa" width="600" />


# Et quoi d'autre ?

On se fait plaisir au travers de cet évènement, il n'y a pas de raison que l'on ne se fasse pas plaisir sur le site du DevFest. Vous verrez les nouveautés que nous allons intégrer au site d'ici au 28 Septembre (et même après...)
 
Si vous êtes intéressé, que vous souhaitez contribuer, n'hésitez pas, la communauté est très ouverte !

**PS** : Au cours de la rédaction de cet article, j'ai constaté un bug dans le projet Hoverboard ce qui m'a permis de faire une [contribution](https://github.com/gdg-x/hoverboard/pull/257) ✔️