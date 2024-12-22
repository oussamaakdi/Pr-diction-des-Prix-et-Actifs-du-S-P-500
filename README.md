<!DOCTYPE html>
<html>
<head>
    <title>Prédiction des Prix et Actifs du S&P 500 avec Machine Learning</title>
</head>
<body>
    <h1 align="center">Prédiction des Prix et Actifs du S&P 500 avec Machine Learning</h1>
    
    <p>
        Ce projet explore l'utilisation de diverses techniques de Machine Learning pour prédire les prix de clôture logarithmiques (<i>Log_Close</i>) de l'indice <b>S&P 500</b>. L'objectif est de fournir des outils permettant d'orienter des stratégies d'investissement sur cet indice de référence, en s'appuyant sur des données financières et économiques enrichies.
    </p>

    <h2>🔍 Contexte</h2>
    <p>
        Le <b>S&P 500</b> est un indice regroupant les 500 plus grandes entreprises cotées aux États-Unis, servant de baromètre clé pour mesurer la santé économique et les performances globales du marché. Ce projet combine des données historiques du S&P 500 avec des indicateurs macroéconomiques et techniques pour construire des modèles prédictifs robustes.
    </p>

    <h2>🎯 Objectifs</h2>
    <ul>
        <li>Analyser les tendances historiques des prix et des indicateurs économiques.</li>
        <li>Développer plusieurs modèles de prédiction, incluant des modèles linéaires, des algorithmes basés sur les arbres de décision et des réseaux neuronaux récurrents.</li>
        <li>Évaluer les performances des modèles en termes de précision et de robustesse.</li>
        <li>Proposer des stratégies d’investissement basées sur les résultats des modèles.</li>
    </ul>

    <h2>🛠️ Méthodologie</h2>
    <ol>
        <li><b>Collecte des données :</b> Utilisation d'APIs telles que <b>Yahoo Finance</b>, <b>FRED</b>, et <b>Alpha Vantage</b> pour récupérer les données financières et macroéconomiques.</li>
        <li><b>Transformation des données :</b> Application de transformations log pour stabiliser les variations des prix et création de variables techniques telles que RSI et MACD.</li>
        <li><b>Modélisation :</b> Entraînement et évaluation des modèles suivants :
            <ul>
                <li>Régression linéaire</li>
                <li>ARIMA</li>
                <li>Random Forest</li>
                <li>Gradient Boosting</li>
                <li>Réseaux neuronaux LSTM</li>
            </ul>
        </li>
        <li><b>Évaluation :</b> Utilisation de métriques comme le R² et le MSE pour comparer les performances des modèles.</li>
    </ol>

    <h2>📊 Résultats</h2>
    <ul>
        <li>La <b>régression linéaire</b> a montré une capacité explicative limitée (R² = 0.177) mais a révélé des relations significatives, notamment avec les variables <i>VIX</i> et <i>Log_RealGDP</i>.</li>
        <li>Le modèle <b>ARIMA</b> (ARIMA(2, 0, 0)) a capturé efficacement les dépendances temporelles à court terme, mais reste limité pour des variations complexes.</li>
        <li>Les modèles basés sur les arbres (<b>Random Forest</b>, <b>Gradient Boosting</b>) ont montré des performances faibles, suggérant un besoin de variables explicatives plus pertinentes.</li>
        <li>Le modèle <b>LSTM</b> s’est distingué par sa capacité à capturer les tendances principales, bien qu'il puisse encore être amélioré avec des ajustements d’hyperparamètres.</li>
    </ul>

    <h2>📈 Stratégies d'investissement</h2>
    <p>
        Les prédictions issues des modèles peuvent orienter des décisions d'investissement :
    </p>
    <ul>
        <li>Utilisation du <b>VIX</b> pour identifier les périodes de forte volatilité.</li>
        <li>Exploitation des modèles <b>LSTM</b> et <b>ARIMA</b> pour anticiper les tendances à long terme et optimiser les décisions d'achat/vente.</li>
    </ul>

    <h2>🔮 Recommandations pour l'avenir</h2>
    <ul>
        <li>Intégrer davantage de données sectorielles et des indicateurs de sentiment pour améliorer les modèles.</li>
        <li>Explorer des architectures avancées, telles que les réseaux LSTM bidirectionnels ou hybrides.</li>
        <li>Tester les modèles sur des indices ou secteurs différents pour évaluer leur généralisabilité.</li>
    </ul>

    <h2>📁 Structure du projet</h2>
    <ul>
        <li><b>data/</b> : Contient les données brutes et transformées.</li>
        <li><b>notebooks/</b> : Scripts et notebooks pour les analyses.</li>
        <li><b>models/</b> : Modèles entraînés et résultats associés.</li>
        <li><b>visualizations/</b> : Graphiques et visualisations des prédictions.</li>
    </ul>

    <h2>⚙️ Installation et Exécution</h2>
    <pre>
    # Cloner le dépôt
    git clone https://github.com/username/sp500-prediction.git
    cd sp500-prediction

    # Installer les dépendances
    pip install -r requirements.txt

    # Lancer le projet
    python main.py
    </pre>

    <h2>📝 Auteurs</h2>
    <p>Développé par [Votre Nom], étudiant en Data Science et Machine Learning.</p>
</body>
</html>


