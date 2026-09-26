# perimeter-site

Pages publiques minimales de Perimeter (outil personnel de Martin Pavloff), requises par Google pour publier l'app OAuth du projet Google Cloud `perimeter` :

- `index.html` — page d'accueil de l'application
- `privacy.html` — règles de confidentialité

Publiées via GitHub Pages : https://realcoolclint.github.io/perimeter-site/

Repo volontairement séparé du repo `perimeter` : ces liens doivent rester en ligne même si `perimeter` repasse en privé (question D29).

## Keep-alive Supabase

`.github/workflows/supabase-keepalive.yml` fait une lecture minimale quotidienne dans la base Supabase de Perimeter, pour éviter la mise en pause du free tier après 7 jours d'inactivité. Secret requis : `SUPABASE_ANON_KEY` (clé publique « anon », jamais la clé `service_role`).

Attention : GitHub suspend les tâches planifiées d'un repo public sans aucune activité pendant 60 jours (un e-mail prévient avant) — il suffit alors de les réactiver dans l'onglet Actions.
