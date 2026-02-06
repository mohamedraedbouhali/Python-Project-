<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eco-Traffic Seattle</title>
    <style>
        :root {
            --primary-color: #2ecc71;
            --secondary-color: #27ae60;
            --dark-bg: #1a1a1a;
            --card-bg: #2d2d2d;
            --text-light: #f4f4f4;
            --accent-color: #3498db;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            background-color: var(--dark-bg);
            color: var(--text-light);
            margin: 0;
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            background: var(--card-bg);
            padding: 40px;
            border-radius: 12px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
        }

        header {
            text-align: center;
            border-bottom: 2px solid var(--primary-color);
            padding-bottom: 20px;
            margin-bottom: 30px;
        }

        h1 { color: var(--primary-color); margin-bottom: 10px; }
        h2 { color: var(--accent-color); font-weight: 300; }
        h3 { color: var(--text-light); opacity: 0.9; }
        h4 { color: var(--primary-color); margin-top: 25px; border-left: 4px solid var(--primary-color); padding-left: 10px; }

        .team-section {
            background: rgba(46, 204, 113, 0.1);
            padding: 15px;
            border-radius: 8px;
            text-align: center;
            margin-bottom: 30px;
        }

        .grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-top: 20px;
        }

        .card {
            background: rgba(255,255,255,0.05);
            padding: 20px;
            border-radius: 8px;
            border: 1px solid rgba(255,255,255,0.1);
        }

        ul { list-style-type: none; padding: 0; }
        li { margin-bottom: 10px; padding-left: 25px; position: relative; }
        li::before { content: "➔"; position: absolute; left: 0; color: var(--primary-color); }

        .tech-tag {
            display: inline-block;
            background: var(--secondary-color);
            color: white;
            padding: 2px 8px;
            border-radius: 4px;
            font-size: 0.85em;
            margin: 2px;
        }

        footer {
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #444;
        }

        .deliverables {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 10px;
        }

        .badge {
            background: #444;
            padding: 10px 20px;
            border-radius: 20px;
            font-size: 0.9em;
            border: 1px solid var(--primary-color);
        }
    </style>
</head>
<body>

<div class="container">
    <header>
        <h1>Eco-Traffic Seattle</h1>
        <h3>Prédiction des Niveaux de Congestion par Enrichissement de Données</h3>
    </header>

    <div class="team-section">
        <p>Created by</p>
        <h3>Mohamed Raed Bouhali & Ilef Ben Hassen</h3>
    </div>

    <section>
        <h4>1. Présentation du Projet</h4>
        <p><strong>Titre :</strong> SmartTraffic Seattle : Système de Prédiction de Congestion Urbaine par Enrichissement Multisources.</p>
        <p><strong>Contexte :</strong> Dans le cadre du module <em>"Python for Data Science 2"</em>, ce projet vise à transformer des données statiques de comptage de véhicules en un outil prédictif dynamique.</p>
        <p><strong>Objectif :</strong> Prédire le niveau de trafic (Fluide, Modéré, Critique) en combinant des données historiques et contextuelles (Météo/News).</p>
    </section>

    <section>
        <h4>2. Spécifications Fonctionnelles</h4>
        <div class="grid">
            <div class="card">
                <strong>[Data Ingestion]</strong>
                <p>Collecte automatisée des données météo 2022 et extraction d'incidents via Web Scraping.</p>
            </div>
            <div class="card">
                <strong>[Predictive Core]</strong>
                <p>Classification du niveau de trafic basée sur les caractéristiques géospatiales et temporelles.</p>
            </div>
            <div class="card">
                <strong>[User Interface]</strong>
                <p>Visualisation interactive sur un Dashboard React avec cartographie dynamique.</p>
            </div>
            <div class="card">
                <strong>[Service Access]</strong>
                <p>Exposition des prédictions via une API REST FastAPI.</p>
            </div>
        </div>
    </section>

    <section id="technical-stack">
        <h4>3. Spécifications Techniques</h4>
        
        <h3>🛠 A. Data Pipeline & ML</h3>
        <ul>
            <li><strong>Sources :</strong> Fichier trafficFlow.csv (SDOT) + BeautifulSoup/Selenium.</li>
            <li><strong>Prétraitement :</strong> Feature Engineering (saisonnalité, heures de pointe).</li>
            <li><strong>Équilibrage :</strong> Algorithme <span class="tech-tag">SMOTE</span> pour les classes minoritaires.</li>
            <li><strong>Modélisation :</strong> Random Forest vs XGBoost avec <span class="tech-tag">GridSearchCV</span>.</li>
            <li><strong>Gouvernance :</strong> Suivi via <span class="tech-tag">MLflow</span>.</li>
        </ul>

        <h3>🌐 B. Architecture & Déploiement</h3>
        <ul>
            <li><strong>Backend :</strong> FastAPI (Endpoints unitaire & batch).</li>
            <li><strong>Frontend :</strong> React (Vite) + Leaflet.js.</li>
            <li><strong>DevOps :</strong> Docker & Docker-Compose.</li>
        </ul>
    </section>

    <footer>
        <h4>📌 Livrables Attendus</h4>
        <div class="deliverables">
            <div class="badge">📂 Code Source GitHub</div>
            <div class="badge">🐳 Environnement Docker</div>
            <div class="badge">📊 Dashboard Live</div>
        </div>
    </footer>
</div>

</body>
</html>
