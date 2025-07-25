## ![🕸️](https://fonts.gstatic.com/s/e/notoemoji/16.0/1f578_fe0f/32.png) **1. ByteSpider** _(Tiny Web Scraper & Recon)_

> **Mission :**  
> Développe un web crawler capable de récupérer des pages, d’extraire des liens et de détecter des patterns.  
> Utilise-le pour cartographier le site de test en local.

#### **Consignes :**

- Crée un script python qui explore un site à partir d’une URL de départ.
- Récupère tous les liens.
- Cherche des patterns intéressants (emails et num de tel).
- Génère un rapport de reconnaissance (infos trouvées).

**Cible** : Site de test en LOCAL

#### Site de test :

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Page de test ByteSpider</title>
</head>
<body>
    <h1>Bienvenue sur la page de test de ByteSpider</h1>

    <h2>Emails</h2>
    <ul>
        <li>john.doe@example.com</li>
        <li>contact@entreprise.fr</li>
        <li>admin@site.co.uk</li>
        <li>mauvais@mail</li>
        <li>nom@@faux.com</li>
        <li>pasunemail.com</li>
        <li>valid.user@sub.domain.fr</li>
    </ul>

    <h2>Numéros de téléphone</h2>
    <ul>
        <li>01 23 45 67 89</li>
        <li>06 12 34 56 78</li>
        <li>+33 1 23 45 67 89</li>
        <li>+33 6 12 34 56 78</li>
        <li>07-12-34-56-78</li>
        <li>+33612345678</li>
        <li>0612345678</li>
        <li>032045123</li>
        <li>not a number: 123-abc-456</li>
    </ul>

    <h2>Liens internes</h2>
    <ul>
        <li><a href="/page1">Page 1</a></li>
        <li><a href="/page2">Page 2</a></li>
        <li><a href="/produits/article-123">Article 123</a></li>
        <li><a href="/contact">Contact</a></li>
    </ul>

    <h2>Liens externes</h2>
    <ul>
        <li><a href="https://example.com">Site exemple</a></li>
        <li><a href="https://github.com">GitHub</a></li>
    </ul>
</body>
</html>
```
