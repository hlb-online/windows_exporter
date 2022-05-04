# windows_exporter, HLB fork

A Prometheus exporter for Windows machines.

## Repository structure

The default branch, `cicd`, only contains GitHub Actions definitions to sync, rebase and build other branches.

On the `upstream` branch, changes from the https://github.com/prometheus-community/windows_exporter repository are synced
periodically. This branch is therefore always an exact mirror of `prometheus-community/windows_exporter`s `master` branch.

Our changes and custom collectors are kept on the `main` branch. This branch is periodically rebased onto `upstream` so
it's always based on the latest available windows_exporter release.

The `main` branch should also have artifacts and releases built regularly, however that's not implemented yet.
