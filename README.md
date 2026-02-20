# Système Intelligent de Gestion du Trafic (SIGT)

## 🔹 Problématique

Chaque route est conçue pour supporter un certain volume de trafic.  
Lorsque le nombre de véhicules augmente, le réseau routier doit être amélioré pour éviter la congestion.  

Cependant :  
- Améliorer le réseau routier peut être difficile, irréalisable ou impossible.  
- Il n’est pas possible de surveiller chaque route depuis tous les points, ce qui crée des **angles morts**.  

Le projet vise donc à fournir un **système intelligent capable de détecter et prédire la congestion** à partir de vidéos de surveillance en temps réel.

---

## 🔹 Objectifs

- Détecter et compter les véhicules sur les routes à l’aide de modèles de deep learning (YOLO, Faster-RCNN).  
- Mesurer le niveau de congestion en temps réel.  
- Fournir des alertes ou statistiques pour aider à la gestion du trafic.  
- Permettre la visualisation et l’export de résultats (vidéos annotées, statistiques).

---

## 🔹 Architecture du projet

### Diagramme Mermaid

```mermaid
graph TD
    A[Caméras de surveillance / Vidéos] --> B[Pré-traitement des images]
    B --> C[Détection de véhicules]
    C --> D[Analyse de congestion]
    D --> E[Export / Visualisation]

