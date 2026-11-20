# AGENTS.md

OAM app-model repo — `oam-application-definition.yml` is the deployable
projection of one application; every field is validated by `orch-ci` and
consumed by `topo-deploy.py` (`progmise/reusable-workflows@v1`). Never
store secret values here: `*Id` fields only name consumer-repo
secrets/variables. Single protected `main` branch — work lands via
`<type>/<snake_description>` + PR.
