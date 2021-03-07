<p align="center">
  <img src="https://user-images.githubusercontent.com/48243955/110245806-0a875d80-7f65-11eb-933e-8ecb9b1ded93.png" />
</p>

# Liste (travail en cours) d'outils liés à l'accessibilité pour les développeurs

> La liste n'a pas vocation à être exhaustive (mais vous pouvez proposer des ajouts / mise à jour) et est orientée **développeur web**.

> Les liens sont majoritairement anglophones j'ai donc choisi de préciser lorsqu'ils étaient disponibles en français 

Dernière mise à jour - 06/03/2021

---

- [Liste (travail en cours) d'outils liés à l'accessibilité pour les développeurs](#Liste-travail-en-cours-doutils-li%C3%A9s-%C3%A0-laccessibilit%C3%A9-pour-les-d%C3%A9veloppeurs)
  - [Apprentissage / Documentations](#Apprentissage--Documentations)
    - [Guidelines et réglementations](#Guidelines-et-r%C3%A9glementations)
    - [Listes de documentations utiles](#Listes-de-documentations-utiles)
  - [Checklists](#Checklists)
  - [Extensions pour navigateurs web, et bookmarklets](#Extensions-pour-navigateurs-web-et-bookmarklets)
    - [Les leaders](#Les-leaders)
    - [Autres outils utiles](#Autres-outils-utiles)
  - [Outils proposant une intégration dans une CI](#Outils-proposant-une-int%C3%A9gration-dans-une-CI)
  - [Exemples de code, librairies et templates](#Exemples-de-code-librairies-et-templates)
  - [Tester par d'autres moyens](#Tester-par-dautres-moyens)
  - [TODO - Les choses à ne pas faire](#TODO---Les-choses-%C3%A0-ne-pas-faire)
  - [Divers](#Divers)


## Apprentissage / Documentations

### Guidelines et réglementations
* [WCAG 2.0 Guidelines](https://www.w3.org/TR/WCAG20/#guidelines) - Liste des guidelines du WCAG (W3C Accessiblity Guidelines).

* [WAI - Stories of Web Users](https://www.w3.org/WAI/people-use-web/user-stories/) - Liste de personas d'utilisateurs du web avec divers handicaps proposée par le WAI (Web Accessibility Initiative, part of W3C). Chacun des personas réfèrence des liens vers les sections concernées des guidelines du WAI.

* [RGAA - numerique.gouv.fr (fr)](https://www.numerique.gouv.fr/publications/rgaa-accessibilite/) - Site du gouvernement pour le Référentiel Général d'Amélioration de l'Accessibilité).
* [RGAA - critères et tests (fr)](https://www.numerique.gouv.fr/publications/rgaa-accessibilite/methode-rgaa/criteres/) - Liste des critères et tests du RGAA.


> https://www.w3.org/WAI/ER/tools/

### Listes de documentations utiles

* [Tutoriels d'accessibilité Web du W3C](https://www.w3.org/WAI/tutorials/)

* [How to Meet WCAG requirements (Quick Reference)](https://www.w3.org/WAI/WCAG21/quickref/) -  Outil du W3C sous forme de liste filtrable des recommandations du WCAG Guidelines et les techniques pour y faire face. 

* [A11y Project ressources](https://www.a11yproject.com/resources/) - Le A11y Project (projet communautaire) propose une liste de ressources liées à l'accessibilité (dont une checklist, voir plus bas) telle que des ouvrages et articles, des outils etc.

* [A11y styleguide](https://a11y-style-guide.com/style-guide/section-resources.html) - Liste de ressources concernant l'implementation de l'accessibilité, comprenant des explications et des exemples de code.

* [HTML5 accessibility support by browsers](https://www.html5accessibility.com/)

* [A11yCoffee](https://a11y.coffee/)

## Checklists

* [Checklist A11y project](https://www.a11yproject.com/checklist/) - Checklist des recommandations WCAG pouvant servir d'exemple et fournie par le A11y Project.

* [Checklist Pidila](https://pidila.gitlab.io/checklist-pidila/?R%C3%A9f%C3%A9rentiel=RGAA&Profil=D%C3%A9veloppement) - Checklist du Pidila. Une ressource très utile pour les sites soumis à la RGAA. LA DILA propose aussi une librairie de composants réutilisables et conformes à la réglementation (cf. exemples de code).
* [Checklist US gov](https://accessibility.digital.gov/front-end/getting-started/) - Checklist du gouvernement américain - partie développeur frontend.

## Extensions pour navigateurs web, et bookmarklets

### Les leaders
* [Lighthouse (Chrome)](https://developers.google.com/web/tools/lighthouse) - Lighthouse (Google)est une extension pré-installée sur Chrome et qui fournit plusieurs types d'audit d'une page web notamment l'accessibilité, les bonnes pratiques et la performance.
* [Wave (Chrome/Firefox)](https://wave.webaim.org/extension/) - Wave est une outil proposé par WebAIM (association travaillant sur l'accessibilité du web). Il est disponible sur Chrome et Firefox, et fournit un résumé de différents éléments d'accessibilité directement sur la page web auditée. Wave permet aussi de désactiver les styles CSS.
* [Axe (Chrome/Firefox)](https://www.deque.com/axe/browser-extensions/) - Axe est un outil de la société Deque. Il propose notamment une extension qui s'intégre aux côtés de lightouse (sur chrome) dans les outils de développement et qui permet d'auditer des pages web.

### Autres outils utiles
> Note: les bookmarklets sont des scripts javascript qui peuvent être executés depuis un signet. Ils ne nécessitent donc pas d'installation. 
* [Pa11y](https://github.com/pa11y/pa11y) - Outil d'automatisation de tests d'accessibilité disponible en CLI ou en package node. Peut être utilisé avec Axe.
  * [Koa11y](https://open-indy.github.io/Koa11y/) - Application desktop (Windows, OSX et Linux) utilisant Pa11y.
* [tota11y](https://khan.github.io/tota11y/) - Bookmarklet fourni par la Khan Academy ([Github](https://github.com/Khan/tota11y)) mettant en avant les manquements aux guidelines WCAG d'une page web.
* [HTML_CodeSniffer](https://squizlabs.github.io/HTML_CodeSniffer/) - Bookmarklet  mettant en avant les manquements aux guidelines WCAG d'une page web.
* [A11y.css](https://ffoodd.github.io/a11y.css/) - Disponible sous forme de bookmarklet et d'extension Chrome/Firefox. Met en avant les alertes et erreurs directement sur la page web (overlay).
* [eslint-plugin-jsx-a11y](https://github.com/jsx-eslint/eslint-plugin-jsx-a11y) - Plugin eslint permettant la vérification de l'accessibilité sur du code React.
* [Images On/Off (Chrome)](https://chrome.google.com/webstore/detail/images-onoff/nfmlhilnjccdggifdbhnhkffmjgalbgg) - Extension Chrome permettant de désactiver toutes les images d'un site pour tester le comportement.

## Outils proposant une intégration dans une CI

* [Lighthouse CI](https://github.com/GoogleChrome/lighthouse-ci/blob/main/docs/getting-started.md) - Voir plus haut pour une description de Lighthouse. L'outil s'intégre aussi dans une CI et est compatible avec la plupart des providers du marché(Github Actions, Travis CI, Circle CI, Gitlab CI,...).

* [Axe core](https://www.deque.com/axe/browser-extensions/) - TODO

* [Pa11y CI](https://github.com/pa11y/pa11y-ci) - Pa11y CI est un utilitaire de tests d'accessibilité s'intégrant à une CI, et basé sur [Pa11y](https://github.com/pa11y/pa11y).

* [Asqatasun](https://asqatasun.org/) - TODO

## Exemples de code, librairies et templates

* [Van11y](https://van11y.net/) - Collection de scripts accessibles pour des Rich Interfaces Elements tels que des modal, tooltips etc. et utilisant les guidelines ARIA.

* [inclusive-components.design](https://inclusive-components.design/) - Librairies de patterns accessible avec exemple de *inclusive components* (tels que todolist, image slider) avec des explications et des exemples de code.

* [Accessible components](https://github.com/scottaohara/accessible_components) - Repository (Github) avec des exemples de composants accessibles (js) et des explications (MIT licence). Du même auteur: [The Accessibility of Styled Form Controls
](https://github.com/scottaohara/a11y_styled_form_controls).

* [Deque University code library (beta)](https://dequeuniversity.com/library/) - Deque (concepteur de l'outil Axe) fournit une liste de composants accessibles (code source + référence aux guidelines WCAG).

## Tester par d'autres moyens

* [VoiceOver - WebAIM](https://webaim.org/articles/voiceover/) - Ressource de WebAIM expliquant comme utiliser VoiceOver pour vérifier l'accessibilité d'un web site.

## TODO - Les choses à ne pas faire

> Ressources sur les choses à challenger en tant que dev (personnaliser les inputs etc.)

## Divers

* [a11y-nutrition-cards](https://davatron5000.github.io/a11y-nutrition-cards/#tooltip) - visualisation simplifiée des attentes en terme d'accessibilité sur certains types de composants (button, tabs, ...)
