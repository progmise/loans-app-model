# <application>-app-model

OAM application model — oam-application-definition.yml declares the released set of components (repo + version + needs + infra bindings) deployable together, plus environments and promotion trails. Generated from oam-app-model-template.

Flow: PR bumping metadata.version → ci.yml (orch-ci validates) → merge → release.yml drafts Release v<version> → publish to approve → deploy.yml (orch-deploy topo-sorts + dispatches each consumer, needs ORCHESTRATOR_TOKEN).
