# Bundle vs core image verification: 1.23.3

**Generated:** 2026-10-25 13:57 IST
**Verdict:** PASS

**Bundle snapshot:** `openshift-pipelines-bundle-1-23-20261024-113334-000`
**Bundle created:** 2026-10-24 17:07 IST
**Bundle image:** `quay.io/redhat-user-workloads/tekton-ecosystem-tenant/pipelines-operator-bundle@sha256:8c6a5eeb36272ed40a1b4771ab9f319b23ae0c3583649befbdefd167e22efe9c`
**Operator revision:** `2e2fd0c57b27207b225d3861aaa7b25bc31a2bcd`
**Core snapshot:** `openshift-pipelines-core-1-23-20261024-111413-000-tt`
**Core created:** 2026-10-24 16:54 IST

The bundle snapshot records operator commit `2e2fd0c57b27207b225d3861aaa7b25bc31a2bcd`. The CSV and `project.yaml` at that commit were compared with every component image in the core snapshot. A match requires the same image name and the same sha256 digest. The CSV publishes each digest on `registry.stage.redhat.io/openshift-pipelines`. `project.yaml` keeps the Konflux reference on `quay.io/redhat-user-workloads/tekton-ecosystem-tenant`.

## Summary

| Check | Result |
| --- | --- |
| Core components checked | 40 |
| Digest match in CSV relatedImages, deployment references, and project.yaml | 40 |
| Mismatch or missing | 0 |
| Staging relatedImages with no core component | 0 |
| CSV env values that differ from the same relatedImage | 0 |
| quay.io references left in the CSV | 0 |

All 40 core snapshot images are present in this bundle. Each digest matches, and every OpenShift Pipelines image in the CSV is on the staging registry.

## Core component images

| Component | Image | Digest | CSV names | Status |
| --- | --- | --- | --- | --- |
| `console-plugin-1-23-console-plugin` | `pipelines-console-plugin-rhel9` | `sha256:12064cb8e105538bc3309ec520ac51669e73f7a7033e8b8d7132ae103fd6508f` | `IMAGE_PIPELINES_CONSOLE_PLUGIN` | MATCH |
| `console-plugin-pf5-1-23-console-plugin` | `pipelines-console-plugin-pf5-rhel9` | `sha256:2e7a4796afda890dfa78e4bec5016d72a27a56555e4a436baeb34fedff22fb54` | `IMAGE_PIPELINES_CONSOLE_PLUGIN_LEGACY` | MATCH |
| `manual-approval-gate-1-23-controller` | `pipelines-manual-approval-gate-controller-rhel9` | `sha256:b0aeb566672486bd01a539ee9d1bd6288a7c284a140cb97fa0e58c340f3f5168` | `IMAGE_MAG_TEKTON_TASKGROUP_CONTROLLER` | MATCH |
| `manual-approval-gate-1-23-webhook` | `pipelines-manual-approval-gate-webhook-rhel9` | `sha256:0c5c3f68f25b235e1b8c89425cc51ff2758792678b8f127152b5b8bd6aca4307` | `IMAGE_MAG_MANUAL_APPROVAL` | MATCH |
| `multicluster-proxy-aae-1-23-multicluster-proxy-aae` | `pipelines-multicluster-proxy-aae-rhel9` | `sha256:97f5277f8e19f380d9236d69ae49be6bd79cbaaaa72c45a191b866f633ccb187` | `IMAGE_MULTICLUSTERPROXYAAE_PROXY_AAE` | MATCH |
| `opc-1-23-opc` | `pipelines-opc-rhel9` | `sha256:a306bdb7d050632d01f80fc168e6117d1bbb57148bec57bd1e2413ad3d10bd07` | `IMAGE_ADDONS_OPC` | MATCH |
| `operator-1-23-operator` | `pipelines-rhel9-operator` | `sha256:1c85273080bba86356853a87d70b237c3c60c31c63f63cd289cb3e984eaae6ba` | `OPENSHIFT_PIPELINES_OPERATOR_CLUSTER_OPERATIONS`, `OPENSHIFT_PIPELINES_OPERATOR_LIFECYCLE` | MATCH |
| `operator-1-23-proxy` | `pipelines-operator-proxy-rhel9` | `sha256:09396131870b54566339bbac160e166df580488703ead25922fa6e6efba84e4a` | `IMAGE_PIPELINES_PROXY` | MATCH |
| `operator-1-23-webhook` | `pipelines-operator-webhook-rhel9` | `sha256:69a48c23ca91279a88f6bdf1f7c693b8efa945295c7f77f5532d7feaf0312a37` | `TEKTON_OPERATOR_WEBHOOK` | MATCH |
| `pipelines-as-code-1-23-cli` | `pipelines-pipelines-as-code-cli-rhel9` | `sha256:fc1521a88497413850672b4f3f8347f0fff768e6799fb0a282ae77f9e22a0c55` | `IMAGE_PAC_PAC_CLI` | MATCH |
| `pipelines-as-code-1-23-controller` | `pipelines-pipelines-as-code-controller-rhel9` | `sha256:24e95e216048a393de7429956f5fb44c4ca505172f39fa35c7f77672b70b2d84` | `IMAGE_PAC_PAC_CONTROLLER` | MATCH |
| `pipelines-as-code-1-23-watcher` | `pipelines-pipelines-as-code-watcher-rhel9` | `sha256:2874a4846b07c586258790695c7e9ea9e942b05747ff287aa2efb23b6f10c1e3` | `IMAGE_PAC_PAC_WATCHER` | MATCH |
| `pipelines-as-code-1-23-webhook` | `pipelines-pipelines-as-code-webhook-rhel9` | `sha256:39fe49e35c823a55d290de11296d4107561743491da3a94a15eda20597717ca8` | `IMAGE_PAC_PAC_WEBHOOK` | MATCH |
| `serve-tkn-cli-1-23-serve-tkn-cli` | `pipelines-serve-tkn-cli-rhel9` | `sha256:1c13cfa5a7371466e67acb8bedf8e73ef3b3930ff92fe1bd6b31f107d7a21efe` | `IMAGE_ADDONS_TKN_CLI_SERVE`, `IMAGE_ADDONS_TKN_CLI_SERVE_INIT_CONFIG` | MATCH |
| `syncer-service-1-23-syncer-service` | `pipelines-syncer-service-rhel9` | `sha256:f3fa30656b5268e6d748c146fc1e8cf75675c4a50ee1dd4b7feed5195d7ee2c8` | `IMAGE_SYNCER_SERVICE_WORKLOAD_CONTROLLER` | MATCH |
| `tekton-caches-1-23-cache` | `pipelines-cache-rhel9` | `sha256:dbd0d4ff381ea35731f77e17b92f3ecce693c37486ef61704726712f9e6903bc` | `IMAGE_ADDONS_CACHE_FETCH`, `IMAGE_ADDONS_CACHE_UPLOAD` | MATCH |
| `tekton-kueue-1-23-scheduler` | `pipelines-scheduler-rhel9` | `sha256:7d0afab498e2aec1143053557c38379da8d60b5680b46f439a75fe8b0f6c5e1c` | `IMAGE_SCHEDULER_MANAGER`, `IMAGE_SCHEDULER_WEBHOOK` | MATCH |
| `tektoncd-chains-1-23-controller` | `pipelines-chains-controller-rhel9` | `sha256:278a287460434cb92c71fca3dfd28904b423bd6f98762f1817096c4e462455f3` | `IMAGE_CHAINS_TEKTON_CHAINS_CONTROLLER` | MATCH |
| `tektoncd-cli-1-23-tkn` | `pipelines-cli-tkn-rhel9` | `sha256:d6ee497f0a5c2f9ab389fe4c5004b385da44db166953430eac98f4b2a3a5d425` | `IMAGE_ADDONS_PARAM_TKN_IMAGE`, `IMAGE_ADDONS_TKN`, `IMAGE_JOB_PRUNER_TKN` | MATCH |
| `tektoncd-git-clone-1-23-git-init` | `pipelines-git-init-rhel9` | `sha256:0391de927c339944887e44186d95aa68212577137b6b97395a07301fad18f56f` | `IMAGE_ADDONS_GIT_CLONE`, `IMAGE_ADDONS_GIT_RUN`, `IMAGE_ADDONS_PARAM_GITINITIMAGE`, `IMAGE_ADDONS_PREPARE_AND_RUN`, `IMAGE_ADDONS_REPORT`, `IMAGE_PIPELINES_ARG__GIT_IMAGE` | MATCH |
| `tektoncd-hub-1-23-api` | `pipelines-hub-api-rhel9` | `sha256:52d243ca04f5918f13587e1054e5b520987b902dd47c348ca5f6a5ee273565e0` | `IMAGE_HUB_TEKTON_HUB_API` | MATCH |
| `tektoncd-hub-1-23-db-migration` | `pipelines-hub-db-migration-rhel9` | `sha256:e52641674e3cac6e026fe2234a2c611086c6c7bdc88e524d1a8cfcc2d4ec6785` | `IMAGE_HUB_TEKTON_HUB_DB_MIGRATION` | MATCH |
| `tektoncd-hub-1-23-ui` | `pipelines-hub-ui-rhel9` | `sha256:9a4bca68de1f201fb39c67bdeddf9f23163b8b45aa2b507a4c880d3790d1096f` | `IMAGE_HUB_TEKTON_HUB_UI` | MATCH |
| `tektoncd-pipeline-1-23-controller` | `pipelines-controller-rhel9` | `sha256:6b6dc5e179f5b4e53de449d50edd7f79ec3544bbfaea10d6d17f5a239bde5392` | `IMAGE_PIPELINES_TEKTON_PIPELINES_CONTROLLER` | MATCH |
| `tektoncd-pipeline-1-23-entrypoint` | `pipelines-entrypoint-rhel9` | `sha256:fd1631cba81ac0d49bb2b84989644c1353eaf2fc44832efce146ab3946a17308` | `IMAGE_PIPELINES_ARG__ENTRYPOINT_IMAGE`, `IMAGE_PIPELINES_ARG__SHELL_IMAGE` | MATCH |
| `tektoncd-pipeline-1-23-events` | `pipelines-events-rhel9` | `sha256:2f7aff11f5bb39b8350579f0a0497b0ea08957b0d8e68fae12e1c05edf7b519b` | `IMAGE_PIPELINES_TEKTON_EVENTS_CONTROLLER` | MATCH |
| `tektoncd-pipeline-1-23-nop` | `pipelines-nop-rhel9` | `sha256:419765a14397e143ac258d9b33958fce7e52cfe3c8109fdb99d2552835e597d8` | `IMAGE_PIPELINES_ARG__NOP_IMAGE` | MATCH |
| `tektoncd-pipeline-1-23-resolvers` | `pipelines-resolvers-rhel9` | `sha256:3b520a7e617ec2bca301d29b653adbec4e2a8220e2597065152ef5a8d0ea551b` | `IMAGE_PIPELINES_CONTROLLER` | MATCH |
| `tektoncd-pipeline-1-23-sidecarlogresults` | `pipelines-sidecarlogresults-rhel9` | `sha256:01201e72dfcfca8cdcf9cfe1b755ea725589848cf86504cd84e63e322251410d` | `IMAGE_PIPELINES_ARG__SIDECARLOGRESULTS_IMAGE` | MATCH |
| `tektoncd-pipeline-1-23-webhook` | `pipelines-webhook-rhel9` | `sha256:62b00ae24f118289f40304dcb91d07d849b7b8075cecd7007f526cd44aa8a148` | `IMAGE_PIPELINES_WEBHOOK` | MATCH |
| `tektoncd-pipeline-1-23-workingdirinit` | `pipelines-workingdirinit-rhel9` | `sha256:083151117caa4ad863ca22b4f9d773c8831ab26ef0fc0e2e4f9ff9f807f17d65` | `IMAGE_PIPELINES_ARG__WORKINGDIRINIT_IMAGE` | MATCH |
| `tektoncd-pruner-1-23-controller` | `pipelines-pruner-controller-rhel9` | `sha256:91102ff21fd63172e33f43a58ec97bd20177ca69a3440df720650032a6f96c62` | `IMAGE_PRUNER_CONTROLLER` | MATCH |
| `tektoncd-pruner-1-23-webhook` | `pipelines-pruner-webhook-rhel9` | `sha256:3191e5fced6a8ee593ca4401b4bb2ddfb76a6a74b18ce7bcc14ff5804523c794` | `IMAGE_PRUNER_WEBHOOK` | MATCH |
| `tektoncd-results-1-23-api` | `pipelines-results-api-rhel9` | `sha256:cde10f57472ea003082b0c19801b0f93365c52d8cb90708e7d94ad772a562908` | `IMAGE_RESULTS_API` | MATCH |
| `tektoncd-results-1-23-retention-policy-agent` | `pipelines-results-retention-policy-agent-rhel9` | `sha256:a607a06161c7de7b193dffd0e50a1a3af807bf337aa6ce6d729cc21a6127bb57` | `IMAGE_RESULTS_RETENTION_POLICY_AGENT` | MATCH |
| `tektoncd-results-1-23-watcher` | `pipelines-results-watcher-rhel9` | `sha256:3a348f3646daf3c3e7cceb1b89554ac3d183313ece3c6a09b7dbd0cc120728a1` | `IMAGE_RESULTS_WATCHER` | MATCH |
| `tektoncd-triggers-1-23-controller` | `pipelines-triggers-controller-rhel9` | `sha256:a70f776b581e6929d5d62d262041f7c5363b3c62a754938fe7e475042dd90a19` | `IMAGE_TRIGGERS_TEKTON_TRIGGERS_CONTROLLER` | MATCH |
| `tektoncd-triggers-1-23-core-interceptors` | `pipelines-triggers-core-interceptors-rhel9` | `sha256:b23a927a8085e16e30984da9a6ec3871d5bde6ebe6bf2a1a7bcd0097b19fa3ca` | `IMAGE_TRIGGERS_TEKTON_TRIGGERS_CORE_INTERCEPTORS` | MATCH |
| `tektoncd-triggers-1-23-eventlistenersink` | `pipelines-triggers-eventlistenersink-rhel9` | `sha256:1ebe5a61ed79ed40393cb92ccbd46e95faa16f02de4c95eda2f49c4a7f2cc0eb` | `IMAGE_TRIGGERS_ARG__EL_IMAGE` | MATCH |
| `tektoncd-triggers-1-23-webhook` | `pipelines-triggers-webhook-rhel9` | `sha256:ccdde2e112273f26a731ac1a973c2c87546a05d023d9fa54cafd794522d71357` | `IMAGE_TRIGGERS_WEBHOOK` | MATCH |

## External images in the bundle

These references are not built by the core snapshot.

| CSV name | Image |
| --- | --- |
| `IMAGE_ADDONS_PARAM_KN_IMAGE` | `registry.redhat.io/openshift-serverless-1/kn-client-kn-rhel9@sha256:aee19896d17a431ba980564fdb73ef08ad1512f586fbdf954cecef6258f7a8df` |
| `IMAGE_ADDONS_KN` | `registry.redhat.io/openshift-serverless-1/kn-client-kn-rhel9@sha256:aee19896d17a431ba980564fdb73ef08ad1512f586fbdf954cecef6258f7a8df` |
| `IMAGE_ADDONS_SKOPEO_COPY` | `registry.redhat.io/rhel9/skopeo@sha256:a106a5e93102e859d5420561af11c3f21930872d2d1cc66a13bd5fe1a799759b` |
| `IMAGE_ADDONS_SKOPEO_RESULTS` | `registry.redhat.io/rhel9/skopeo@sha256:a106a5e93102e859d5420561af11c3f21930872d2d1cc66a13bd5fe1a799759b` |
| `IMAGE_ADDONS_PARAM_BUILDER_IMAGE` | `registry.redhat.io/rhel9/buildah@sha256:ce2db38cddeedde4489473a689981c532dff4e2e63971d20bb7b3ceca996c18d` |
| `IMAGE_ADDONS_BUILD` | `registry.redhat.io/rhel9/buildah@sha256:ce2db38cddeedde4489473a689981c532dff4e2e63971d20bb7b3ceca996c18d` |
| `IMAGE_ADDONS_S2I_BUILD` | `registry.redhat.io/rhel9/buildah@sha256:ce2db38cddeedde4489473a689981c532dff4e2e63971d20bb7b3ceca996c18d` |
| `IMAGE_ADDONS_GENERATE` | `registry.redhat.io/source-to-image/source-to-image-rhel9@sha256:798e0e860df8e3ca1ff5f8aa796940d6dbd4b739ccfc35c6f4c9bc046d5f0c12` |
| `IMAGE_ADDONS_GEN_ENV_FILE` | `registry.redhat.io/source-to-image/source-to-image-rhel9@sha256:798e0e860df8e3ca1ff5f8aa796940d6dbd4b739ccfc35c6f4c9bc046d5f0c12` |
| `IMAGE_ADDONS_S2I_GENERATE` | `registry.redhat.io/source-to-image/source-to-image-rhel9@sha256:798e0e860df8e3ca1ff5f8aa796940d6dbd4b739ccfc35c6f4c9bc046d5f0c12` |
| `IMAGE_ADDONS_MVN_SETTINGS` | `registry.redhat.io/ubi9/ubi-minimal@sha256:c4c285d42941ebb2bd4da878479008e1e4536bb599aad1dbe568f89de9053661` |
| `IMAGE_ADDONS_LOAD_SCRIPTS` | `registry.redhat.io/ubi9/ubi-minimal@sha256:c4c285d42941ebb2bd4da878479008e1e4536bb599aad1dbe568f89de9053661` |
| `IMAGE_ADDONS_MAVEN_GENERATE` | `registry.redhat.io/ubi9/ubi-minimal@sha256:c4c285d42941ebb2bd4da878479008e1e4536bb599aad1dbe568f89de9053661` |
| `IMAGE_ADDONS_PREPARE` | `registry.redhat.io/ubi9/ubi-minimal@sha256:c4c285d42941ebb2bd4da878479008e1e4536bb599aad1dbe568f89de9053661` |
| `IMAGE_HUB_TEKTON_HUB_DB` | `registry.redhat.io/rhel9/postgresql-15@sha256:accc0970a3adaaae64517e3a11dd1012f094edd95b05c0514e529bf94240c76b` |
| `IMAGE_RESULTS_POSTGRES` | `registry.redhat.io/rhel9/postgresql-15@sha256:accc0970a3adaaae64517e3a11dd1012f094edd95b05c0514e529bf94240c76b` |
| `IMAGE_ADDONS_PARAM_MAVEN_IMAGE` | `registry.redhat.io/ubi9/openjdk-17@sha256:716810ec4ad7805f57b6434da9405188cb98b30042bdb1cff0d833f76ed5b4b0` |
| `IMAGE_ADDONS_MAVEN_GOALS` | `registry.redhat.io/ubi9/openjdk-17@sha256:716810ec4ad7805f57b6434da9405188cb98b30042bdb1cff0d833f76ed5b4b0` |
| `IMAGE_ADDONS_OC` | `image-registry.openshift-image-registry.svc:5000/openshift/cli:latest` |

## Repositories with more than one revision in the core snapshot

These repositories contribute more than one git revision inside the core snapshot. The bundle references the image digest of each component, so the revision split is not an image mismatch.

| Repository | Revision | Components |
| --- | --- | --- |
| `openshift-pipelines/p12n-manual-approval-gate` | `1287aff810e09cb9dde60dfca16ae56c4fafb281` | `manual-approval-gate-1-23-webhook` |
| `openshift-pipelines/p12n-manual-approval-gate` | `b16885c197b7c8f85c1eff210f088463b57db573` | `manual-approval-gate-1-23-controller` |
| `openshift-pipelines/tektoncd-hub` | `21b9e5dfb7414a49c66d2dde3c2a08a74e9f7f5d` | `tektoncd-hub-1-23-api`, `tektoncd-hub-1-23-ui` |
| `openshift-pipelines/tektoncd-hub` | `e9c751ef5801bed099a708b74bc1bbea1405d7aa` | `tektoncd-hub-1-23-db-migration` |
| `openshift-pipelines/tektoncd-pipeline` | `a49afe1533447dc35e0dd99767a75722c5af8cc9` | `tektoncd-pipeline-1-23-controller`, `tektoncd-pipeline-1-23-events`, `tektoncd-pipeline-1-23-sidecarlogresults` |
| `openshift-pipelines/tektoncd-pipeline` | `bf8d7edfd04f05828235170f3429571c2bf01c97` | `tektoncd-pipeline-1-23-entrypoint`, `tektoncd-pipeline-1-23-nop`, `tektoncd-pipeline-1-23-resolvers`, `tektoncd-pipeline-1-23-webhook`, `tektoncd-pipeline-1-23-workingdirinit` |

## Source revisions

| Component | Repository | Revision |
| --- | --- | --- |
| `console-plugin-1-23-console-plugin` | `openshift-pipelines/p12n-console-plugin` | `f50a05d7b88d9d239133b2eb4290972a4da83183` |
| `console-plugin-pf5-1-23-console-plugin` | `openshift-pipelines/p12n-console-plugin-pf5` | `4a29da88769753c1f411fd71d3eb7b9e5951eafb` |
| `manual-approval-gate-1-23-controller` | `openshift-pipelines/p12n-manual-approval-gate` | `b16885c197b7c8f85c1eff210f088463b57db573` |
| `manual-approval-gate-1-23-webhook` | `openshift-pipelines/p12n-manual-approval-gate` | `1287aff810e09cb9dde60dfca16ae56c4fafb281` |
| `multicluster-proxy-aae-1-23-multicluster-proxy-aae` | `openshift-pipelines/p12n-multicluster-proxy-aae` | `e8fbc195d17eaa595761316a0cfc005a71cf23b6` |
| `opc-1-23-opc` | `openshift-pipelines/p12n-opc` | `2c59097718fdce7ea53292a4e4ba03e5d68ba503` |
| `operator-1-23-operator` | `openshift-pipelines/operator` | `300e7c94195da36eeb65e1ce35255b5a5de68465` |
| `operator-1-23-proxy` | `openshift-pipelines/operator` | `300e7c94195da36eeb65e1ce35255b5a5de68465` |
| `operator-1-23-webhook` | `openshift-pipelines/operator` | `300e7c94195da36eeb65e1ce35255b5a5de68465` |
| `pipelines-as-code-1-23-cli` | `openshift-pipelines/pac-downstream` | `0a9b02486b34a06746704cbac5d932995d7cf180` |
| `pipelines-as-code-1-23-controller` | `openshift-pipelines/pac-downstream` | `0a9b02486b34a06746704cbac5d932995d7cf180` |
| `pipelines-as-code-1-23-watcher` | `openshift-pipelines/pac-downstream` | `0a9b02486b34a06746704cbac5d932995d7cf180` |
| `pipelines-as-code-1-23-webhook` | `openshift-pipelines/pac-downstream` | `0a9b02486b34a06746704cbac5d932995d7cf180` |
| `serve-tkn-cli-1-23-serve-tkn-cli` | `openshift-pipelines/serve-tkn-cli` | `a8add27e2011fc0591525e483b559ad8c98e0829` |
| `syncer-service-1-23-syncer-service` | `openshift-pipelines/p12n-syncer-service` | `d2b044cbaa5b5b4c41e3089be2bff807a38a5f3b` |
| `tekton-caches-1-23-cache` | `openshift-pipelines/p12n-tekton-caches` | `8b7198dfdd174ac10ad82cab766ddbfa3b145184` |
| `tekton-kueue-1-23-scheduler` | `openshift-pipelines/tekton-kueue` | `bca5833f7088dc10dbf92ddafd4a0f07acfa0f14` |
| `tektoncd-chains-1-23-controller` | `openshift-pipelines/tektoncd-chains` | `323f1afdef2e5dcec7cf6099299e0ad89407bfa2` |
| `tektoncd-cli-1-23-tkn` | `openshift-pipelines/tektoncd-cli` | `742ea5f1c876e1ce4b39e9e0d58548f291652b6b` |
| `tektoncd-git-clone-1-23-git-init` | `openshift-pipelines/tektoncd-git-clone` | `3c3572e6f89c899a857f64b3cfa3adb5ee829a94` |
| `tektoncd-hub-1-23-api` | `openshift-pipelines/tektoncd-hub` | `21b9e5dfb7414a49c66d2dde3c2a08a74e9f7f5d` |
| `tektoncd-hub-1-23-db-migration` | `openshift-pipelines/tektoncd-hub` | `e9c751ef5801bed099a708b74bc1bbea1405d7aa` |
| `tektoncd-hub-1-23-ui` | `openshift-pipelines/tektoncd-hub` | `21b9e5dfb7414a49c66d2dde3c2a08a74e9f7f5d` |
| `tektoncd-pipeline-1-23-controller` | `openshift-pipelines/tektoncd-pipeline` | `a49afe1533447dc35e0dd99767a75722c5af8cc9` |
| `tektoncd-pipeline-1-23-entrypoint` | `openshift-pipelines/tektoncd-pipeline` | `bf8d7edfd04f05828235170f3429571c2bf01c97` |
| `tektoncd-pipeline-1-23-events` | `openshift-pipelines/tektoncd-pipeline` | `a49afe1533447dc35e0dd99767a75722c5af8cc9` |
| `tektoncd-pipeline-1-23-nop` | `openshift-pipelines/tektoncd-pipeline` | `bf8d7edfd04f05828235170f3429571c2bf01c97` |
| `tektoncd-pipeline-1-23-resolvers` | `openshift-pipelines/tektoncd-pipeline` | `bf8d7edfd04f05828235170f3429571c2bf01c97` |
| `tektoncd-pipeline-1-23-sidecarlogresults` | `openshift-pipelines/tektoncd-pipeline` | `a49afe1533447dc35e0dd99767a75722c5af8cc9` |
| `tektoncd-pipeline-1-23-webhook` | `openshift-pipelines/tektoncd-pipeline` | `bf8d7edfd04f05828235170f3429571c2bf01c97` |
| `tektoncd-pipeline-1-23-workingdirinit` | `openshift-pipelines/tektoncd-pipeline` | `bf8d7edfd04f05828235170f3429571c2bf01c97` |
| `tektoncd-pruner-1-23-controller` | `openshift-pipelines/tektoncd-pruner` | `c2a72dfebf31c9c8d9503e8dce4d69fb2f46f9aa` |
| `tektoncd-pruner-1-23-webhook` | `openshift-pipelines/tektoncd-pruner` | `c2a72dfebf31c9c8d9503e8dce4d69fb2f46f9aa` |
| `tektoncd-results-1-23-api` | `openshift-pipelines/tektoncd-results` | `91b79b6c3c8068348c6ced7c380d61526cf06650` |
| `tektoncd-results-1-23-retention-policy-agent` | `openshift-pipelines/tektoncd-results` | `91b79b6c3c8068348c6ced7c380d61526cf06650` |
| `tektoncd-results-1-23-watcher` | `openshift-pipelines/tektoncd-results` | `91b79b6c3c8068348c6ced7c380d61526cf06650` |
| `tektoncd-triggers-1-23-controller` | `openshift-pipelines/tektoncd-triggers` | `9f5aac94545812ae9c671ab36918a0ac177190d6` |
| `tektoncd-triggers-1-23-core-interceptors` | `openshift-pipelines/tektoncd-triggers` | `9f5aac94545812ae9c671ab36918a0ac177190d6` |
| `tektoncd-triggers-1-23-eventlistenersink` | `openshift-pipelines/tektoncd-triggers` | `9f5aac94545812ae9c671ab36918a0ac177190d6` |
| `tektoncd-triggers-1-23-webhook` | `openshift-pipelines/tektoncd-triggers` | `9f5aac94545812ae9c671ab36918a0ac177190d6` |

