# Projet site de garage

## Rôles et fonctionnalités

- **Admin** : gère les utilisateurs.
- **User** : peut créer et gérer des clients, et être affecté à des interventions.
- **Client** : possède un ou plusieurs véhicules.
- **Vehicle** : appartient à un client et possède plusieurs interventions.
- **Intervention** : appartient à un véhicule, est liée à un utilisateur et contient les coûts.

## Données principales

### User

- `id`
- `email`
- `password`
- `firstName`
- `lastName`
- `role`

### Client

- `id`
- autres informations à définir
- `createdByUserId`

### Vehicle

- `id`
- `name`
- année
- kilométrage
- prix (si le véhicule est à vendre)

### Intervention

- `id`
- `vehicleId`
- `assignedUserId`
- `createdByUserId`
- `status`
- `description`
- `laborCost`
- `partsCost`
- `totalCost`
- `date`
