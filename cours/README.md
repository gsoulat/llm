# 🎓 Formation LLM : De Zéro à la Production

**Formation complète sur les Large Language Models (LLMs) avec Ollama et Python**

## 📋 Vue d'ensemble

Cette formation vous guide à travers tous les aspects des LLMs, de la théorie fondamentale au déploiement en production. Chaque module est conçu pour être progressif et pratique.

## 🎯 Objectifs de la formation

- ✅ Comprendre les concepts fondamentaux des LLMs
- ✅ Maîtriser l'API Ollama et les modèles locaux
- ✅ Développer des applications RAG (Retrieval Augmented Generation)
- ✅ Fine-tuner des modèles pour vos besoins spécifiques
- ✅ Créer des agents intelligents avec des outils
- ✅ Évaluer et optimiser les performances
- ✅ Déployer en production de manière robuste

## 📚 Structure du cours

### 🟢 **Module 1 : Introduction aux LLMs**
- **Fichier** : `module1_introduction_llm.py`
- **Type** : Théorique
- **Durée** : 30 min
- **Contenu** :
  - Qu'est-ce qu'un LLM ?
  - Architecture Transformer
  - Types de modèles (taille, spécialisation, licence)
  - Concepts clés (temperature, top-p, context window)
  - Introduction à Ollama

### 🟢 **Module 2 : Premier script avec Ollama**
- **Fichier** : `module2_premier_script.py`
- **Type** : Pratique
- **Durée** : 45 min
- **Prérequis** : Ollama installé
- **Contenu** :
  - Installation et configuration d'Ollama
  - Première requête API
  - Gestion des paramètres (temperature, tokens)
  - Gestion d'erreurs basique

### 🟢 **Module 3 : Chatbot avec mémoire**
- **Fichier** : `module3_chatbot.py`
- **Type** : Pratique
- **Durée** : 1h
- **Contenu** :
  - API `/chat` vs `/generate`
  - Gestion de l'historique de conversation
  - Rôles système et utilisateur
  - Chatbot interactif complet

### 🟢 **Module 4 : Embeddings et similarité**
- **Fichier** : `module4_embeddings_similarite.py`
- **Type** : Théorique + Pratique
- **Durée** : 1h30
- **Contenu** :
  - Concept d'embeddings vectoriels
  - Génération d'embeddings avec Ollama
  - Calcul de similarité (cosinus, euclidienne)
  - Recherche sémantique simple
  - Classification par embeddings
  - Visualisation 2D (optionnel)

### 🟢 **Module 5 : RAG Simple**
- **Fichier** : `module5_rag_simple.py`
- **Type** : Pratique
- **Durée** : 1h30
- **Contenu** :
  - Création d'une base vectorielle avec ChromaDB
  - Indexation de documents
  - Recherche de documents pertinents
  - Génération augmentée simple

### 🟢 **Module 6 : RAG avec LangChain**
- **Fichier** : `module6_rag_langchain.py`
- **Type** : Pratique
- **Durée** : 2h
- **Contenu** :
  - Introduction à LangChain
  - Chains et composants
  - RAG pipeline complet
  - Optimisations et bonnes pratiques

### 🟢 **Module 7 : Fine-tuning**
- **Fichier** : `module7_fine_tuning.ipynb`
- **Type** : Notebook Jupyter
- **Durée** : 2h30
- **Contenu** :
  - Concepts du fine-tuning
  - LoRA (Low-Rank Adaptation)
  - Framework Unsloth
  - Entraînement sur données personnalisées
  - Évaluation du modèle fine-tuné
  - Export au format GGUF

### 🟢 **Module 8 : Agents et outils**
- **Fichier** : `module8_agents_outils.py`
- **Type** : Pratique
- **Durée** : 2h
- **Contenu** :
  - Concept d'agents LLM
  - Création d'outils personnalisés
  - LangChain Tools et Agents
  - Agent avec outils multiples
  - Cas d'usage avancés

### 🟢 **Module 9 : Évaluation et métriques**
- **Fichier** : `module9_evaluation_metriques.py`
- **Type** : Pratique
- **Durée** : 2h
- **Contenu** :
  - Types d'évaluation (automatique, humaine)
  - Métriques de performance (précision, latence)
  - Détection de problèmes (hallucinations, biais)
  - Benchmark de modèles
  - Évaluation spécialisée par tâche

### 🟢 **Module 10 : Déploiement et production**
- **Fichier** : `module10_deploiement_production.py`
- **Type** : Pratique
- **Durée** : 2h30
- **Contenu** :
  - Architecture de production
  - Gestion de modèles avec fallback
  - Cache intelligent
  - Monitoring et métriques
  - Robustesse et retry
  - Checklist de déploiement

## ⚙️ Prérequis techniques

### Installation de base
```bash
# 1. Python 3.8+
python --version

# 2. Ollama
# Téléchargez depuis https://ollama.ai
ollama --version

# 3. Modèles requis
ollama pull llama3.2:latest
ollama pull mxbai-embed-large

# 4. Dépendances Python
pip install requests numpy matplotlib scikit-learn langchain chromadb
```

### Pour le fine-tuning (Module 7)
```bash
# Installation des bibliothèques lourdes (GPU recommandé)
pip install unsloth trl peft accelerate bitsandbytes
```

### Ressources système recommandées
- **RAM** : 8 GB minimum, 16 GB recommandé
- **Stockage** : 10 GB d'espace libre (pour les modèles)
- **GPU** : Optionnel mais recommandé pour le fine-tuning
- **Internet** : Pour télécharger les modèles initialement

## 🚀 Démarrage rapide

1. **Clonez ou téléchargez le cours**
2. **Installez Ollama** depuis [ollama.ai](https://ollama.ai)
3. **Téléchargez les modèles** :
   ```bash
   ollama pull llama3.2:latest
   ollama pull mxbai-embed-large
   ```
4. **Installez les dépendances Python** :
   ```bash
   pip install -r requirements.txt
   ```
5. **Commencez par le Module 1** :
   ```bash
   python module1_introduction_llm.py
   ```

## 📖 Comment utiliser ce cours

### 📋 Progression recommandée
1. **Lisez attentivement** chaque module dans l'ordre
2. **Exécutez le code** et expérimentez avec les paramètres
3. **Faites les exercices** proposés dans chaque module
4. **Adaptez les exemples** à vos propres cas d'usage
5. **Passez au module suivant** seulement quand vous maîtrisez le précédent

### 🎯 Pour chaque module
- ⏱️ **Temps estimé** : Respectez le temps suggéré, ne vous précipitez pas
- 🔧 **Prérequis** : Vérifiez que vous avez tout installé
- 💡 **Objectifs** : Gardez les objectifs en tête pendant l'apprentissage
- 🧪 **Expérimentation** : Modifiez le code pour bien comprendre
- ❓ **Questions** : Notez vos questions pour les approfondir

### 📝 Exercices et projets
Chaque module contient des exercices pratiques. Essayez de :
- Modifier les paramètres et observer les changements
- Adapter les exemples à vos propres données
- Combiner les concepts de plusieurs modules
- Créer vos propres variations

## 🛠️ Structure des fichiers

```
code/
├── README.md                           # Ce fichier
├── module1_introduction_llm.py         # Théorie et concepts
├── module2_premier_script.py           # Premier contact avec Ollama
├── module3_chatbot.py                  # Chatbot avec mémoire
├── module3_memory_examples.py          # Exemples de gestion mémoire
├── module4_embeddings_similarite.py   # Embeddings et recherche
├── module5_rag_simple.py              # RAG basique avec ChromaDB
├── module6_rag_langchain.py           # RAG avancé avec LangChain
├── module7_fine_tuning.ipynb          # Fine-tuning avec Unsloth
├── module8_agents_outils.py           # Agents et outils
├── module9_evaluation_metriques.py    # Évaluation et métriques
├── module10_deploiement_production.py # Déploiement production
├── data/                               # Données d'exemple
│   └── data_a_entrainer.json         # Dataset pour fine-tuning
├── tools/                             # Outils et utilitaires
│   ├── fibonacci.py                   # Exemple d'outil
│   └── tools.py                       # Collection d'outils
└── chroma_db/                         # Base vectorielle ChromaDB
```

## 🎓 Niveaux de difficulté

| Module | Niveau | Description |
|--------|--------|-------------|
| 1-3 | 🟢 **Débutant** | Concepts de base, premiers scripts |
| 4-6 | 🟡 **Intermédiaire** | Embeddings, RAG, LangChain |
| 7-8 | 🟠 **Avancé** | Fine-tuning, agents complexes |
| 9-10 | 🔴 **Expert** | Évaluation, production |

## 💡 Conseils pour réussir

### ✅ Do's (À faire)
- 📖 **Lisez la documentation** d'Ollama et des bibliothèques
- 🧪 **Expérimentez** avec différents modèles et paramètres
- 💾 **Sauvegardez** vos modifications et expérimentations
- 🤝 **Partagez** vos découvertes avec la communauté
- 🔄 **Pratiquez** régulièrement pour retenir les concepts
- 📝 **Documentez** vos apprentissages et cas d'usage

### ❌ Don'ts (À éviter)
- 🚫 **Ne sautez pas** de modules (progression logique)
- 🚫 **Ne copiez pas** sans comprendre
- 🚫 **N'utilisez pas** de modèles trop lourds au début
- 🚫 **N'ignorez pas** les messages d'erreur
- 🚫 **Ne négligez pas** la sécurité en production

## 🔧 Résolution de problèmes

### Problèmes fréquents

**❌ "Ollama n'est pas accessible"**
```bash
# Vérifier qu'Ollama est démarré
ollama list
# Si erreur, démarrer Ollama
ollama serve
```

**❌ "Modèle non trouvé"**
```bash
# Lister les modèles installés
ollama list
# Télécharger un modèle manquant
ollama pull llama3.2:latest
```

**❌ "Erreur d'import Python"**
```bash
# Installer la bibliothèque manquante
pip install [nom_bibliotheque]
```

**❌ "Mémoire insuffisante"**
- Utilisez un modèle plus petit (ex: `llama3.2:1b`)
- Réduisez la taille du contexte
- Fermez d'autres applications

## 🎯 Après la formation

### 🚀 Projets suggérés
1. **Assistant personnel** avec RAG sur vos documents
2. **Chatbot métier** pour votre domaine d'expertise
3. **Système de recommandation** basé sur les embeddings
4. **Outil d'analyse de sentiment** fine-tuné
5. **Agent multi-outils** pour l'automatisation

### 📚 Pour aller plus loin
- **Communauté Ollama** : [GitHub](https://github.com/ollama/ollama)
- **Documentation LangChain** : [docs.langchain.com](https://docs.langchain.com)
- **Papers sur les LLMs** : [Papers With Code](https://paperswithcode.com)
- **Fine-tuning avancé** : [Hugging Face](https://huggingface.co/docs)

## 🤝 Contribution

Ce cours est open source ! N'hésitez pas à :
- 🐛 Signaler des bugs ou erreurs
- 💡 Proposer des améliorations
- 📖 Ajouter des exemples
- 🌍 Traduire le contenu

## 📄 Licence

Ce cours est distribué sous licence MIT. Vous êtes libre de l'utiliser, le modifier et le distribuer.

## 🎉 Bonne formation !

Profitez bien de cette aventure dans le monde des LLMs ! N'hésitez pas à expérimenter et à dépasser le cadre des exercices proposés.

---

**💻 Commencez dès maintenant :**
```bash
python module1_introduction_llm.py
```

**📧 Questions ?** Consultez la documentation ou la communauté Ollama.

**🌟 Bon apprentissage !**