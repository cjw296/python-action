# Changelog

## 3.1.1 (12 Aug 2024)

- Pin to `hynek/build-and-inspect-python-package` v3.0.1

## 3.1.0 (30 Dec 2025)

- Move uv-run usage to v3
- Simplify `check-distribution` install steps so command can be seen in GitHub Actions UI.

## 3.0.0 (30 Dec 2025)

- Replace `uv-run`'s `uv-command` parameter with a `prefix` parameter.
- Upgrade to `astral-sh/setup-uv@v7`.
- Pin `uv-run` action to `v2` in `check-typing` and `run-tests`.
- Add package extras support to `check-distributions` action.
- Improve command visibility in GitHub Actions UI.
- Fix bug where `project-directory` was not passed to `setup-uv`'s `working-directory` parameter.
- Fix bug in `uv-run` action where the tree shown did not us the same `uv` resolution as the 
  sync and run.

## 2.1.0 (27 Dec 2025)

- Remove duplicate `astral-sh/setup-uv@v5` in `check-formating` action.
- Add `project-directory` parameter to all actions that benefit from it.
- Factor out a `uv-run` action from `check-typing` and `run-tests`.
- The actions now have their own CI!

## 2.0.1 (25 Dec 2025)

- Fix bug in coverage file name

## 2.0.0 (21 Dec 2025)

- Remove unused parameters to `check-coverage` action.
- Add `check-typing` action.
- Add `run-tests` action.

## 1.5.1 (28 Apr 2025)

- Show missing lines in the shell when `check-coverage` fails under 100% coverage.

## 1.5.0 (16 Apr 2025)

- Allow tag format to be specified for carthorse action.

## 1.4.0 (16 Apr 2025)

- Add check to ensure IDE files don't end up in `sdist`.
- Remove non-functional test for `CHANGELOG` in `sdist`.

## 1.3.0 (10 Apr 2025)

- Add `check-formatting` action.

## 1.2.0 (2 Apr 2025)

- Add `check-coverage` action.

## 1.1.0 (20 Mar 2025)

- Add `carthorse` action.

## 1.0.0 (5 Mar 2025)

- Initial implementation of the `check-distributions` action.
