# TP d'initiation aux LLM

Dans ce TP, vous allez apprendre les bases de l'IA générative en manipulant et en contrôlant un LLM open-weight ([Qwen3-1.7B](https://huggingface.co/Qwen/Qwen3-1.7B)) exécuté sur le GPU gratuit de Google Colab.

En sortie de ce module, vous serez capable de :
- Expliquer ce qu'est un token, un tokenizer, un *chat template* et une fenêtre de contexte
- Observer ce que calcule réellement un LLM : une distribution de probabilité sur le token suivant
- Distinguer un modèle *base* d'un modèle *instruct*, et utiliser un modèle de raisonnement
- Appliquer les techniques de prompt engineering : system prompt, zero-shot, one-shot, few-shot
- Contrôler la génération (température, top-k, top-p, échantillonnage)
- Évaluer des sorties de LLM (ROUGE, LLM-as-a-judge)
- Obtenir des sorties structurées (JSON validé par Pydantic)
- Construire une application : RAG sur un document avec LangChain, ou agent SQL avec appel d'outils

## Exercices

Répondre aux questions dans le notebook [TP_initiation_llm.ipynb](./TP_initiation_llm.ipynb), en l'ouvrant dans Colab avec le bouton *Open in Colab* en haut du notebook.

La notation prendra également en compte la qualité de votre code et son optimisation.

## Environnement : 100 % gratuit

Aucune dépense n'est nécessaire pour ce TP.

| Besoin | Solution gratuite |
|---|---|
| GPU (principal) | [Google Colab](https://colab.research.google.com) : `Exécution -> Modifier le type d'exécution -> T4 GPU` |
| GPU (si Colab n'a plus de GPU disponible) | [Kaggle Notebooks](https://www.kaggle.com/code) : environ 30 h de GPU par semaine, `Settings -> Accelerator -> GPU T4 x2` |
| LLM sur votre ordinateur | [Ollama](https://ollama.com) ou [LM Studio](https://lmstudio.ai) avec un modèle de 1 à 4 milliards de paramètres |
| API de LLM (optionnel) | Offres gratuites avec limites de débit : [Google AI Studio](https://aistudio.google.com), [Groq](https://console.groq.com), [OpenRouter](https://openrouter.ai) (modèles `:free`) |

Avec les API gratuites :
- ne mettez jamais de clé d'API en clair dans un notebook (utilisez les *Secrets* de Colab) ;
- n'envoyez aucune donnée personnelle ou confidentielle : les offres gratuites peuvent utiliser vos données pour entraîner leurs modèles.
