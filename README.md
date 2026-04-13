# Code promo Prozis, recuperation automatique depuis shopilo.fr

Module Python pour la recuperation automatique de **codes promo Prozis** depuis [shopilo.fr](https://shopilo.fr/reductions/prozis.com). Renvoie les **coupons Prozis** actifs au format JSON, pret a etre integre dans un bot Telegram, une extension de navigateur ou tout autre outil.

**Page live :** [shopilo-fr.github.io/code-promo-prozis](https://shopilo-fr.github.io/code-promo-prozis/)

![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue) ![License MIT](https://img.shields.io/badge/license-MIT-green)

## Installation

```bash
pip install requests beautifulsoup4
git clone https://github.com/shopilo-fr/code-promo-prozis
cd code-promo-prozis
python fetch.py
```

## Exemple de sortie

```json
[
  {
    "store": "Prozis",
    "code": "SHOPILO10",
    "discount": "10%",
    "description": "10% de reduction sur la nutrition sportive",
    "expires": "2026-10-13",
    "source": "https://shopilo.fr/reductions/prozis.com"
  }
]
```

## Coupons Prozis disponibles

| Reduction | Description | Source |
|----------|-----------|-------|
| 10% | 10% de reduction sur la nutrition sportive | [shopilo.fr](https://shopilo.fr/reductions/prozis.com) |

Codes actifs : **[shopilo.fr/reductions/prozis.com](https://shopilo.fr/reductions/prozis.com)**

## Questions frequentes

### Comment utiliser un code promo Prozis ?
Copiez le code depuis le tableau ci-dessus ou depuis [shopilo.fr](https://shopilo.fr/reductions/prozis.com), ajoutez les produits a votre panier sur Prozis et saisissez le code au moment du paiement dans le champ prevu.

### Combien de temps durent les coupons Prozis ?
Chaque coupon a une date d'expiration indiquee dans la colonne "Expiration". Le script fetch.py renvoie uniquement les coupons actifs au moment de l'execution.

### Ou trouver les bons de reduction Prozis les plus recents ?
La page [shopilo.fr/reductions/prozis.com](https://shopilo.fr/reductions/prozis.com) est mise a jour quotidiennement avec les codes promo Prozis, bons de reduction Prozis et coupons promotionnels Prozis les plus recents.

### Le code ne fonctionne pas. Que faire ?
Verifiez la date d'expiration et les conditions (montant minimum de commande, produits eligibles). Certains codes sont valables uniquement sur l'application mobile ou pour la premiere commande.

## A propos de Prozis

Prozis est l'une des boutiques en ligne les plus populaires. Sur [shopilo.fr](https://shopilo.fr/reductions/prozis.com), retrouvez les meilleurs codes promo Prozis, coupons Prozis verifies et bons de reduction Prozis actifs, mis a jour chaque jour.

## Installation npm

```bash
npm install code-promo-prozis
```

```javascript
const { fetchCoupons } = require('code-promo-prozis');
fetchCoupons().then(data => console.log(data));
```

## Licence

MIT, donnees extraites de [shopilo.fr](https://shopilo.fr)
