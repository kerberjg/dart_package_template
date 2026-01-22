# dart_package_template
GitHub template repository for Dart packages, ready for pub.dev publication.

<!-- Badges -->
[![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](LICENSE)
[![build](https://github.com/kerberjg/dart_package_template/actions/workflows/package.yaml/badge.svg)](https://github.com/kerberjg/dart_package_template/actions/workflows/package.yaml)
[![example](https://github.com/kerberjg/dart_package_template/actions/workflows/example.yaml/badge.svg)](https://github.com/kerberjg/dart_package_template/actions/workflows/example.yaml)
[![stars](https://img.shields.io/github/stars/kerberjg/dart_package_template.svg)](https://github.com/kerberjg/dart_package_template/stargazers)

<!-- Pub.dev Badges -->
[![pub package](https://img.shields.io/pub/v/dart_package_template.svg)](https://pub.dev/packages/dart_package_template)
[![pub score](https://img.shields.io/pub/points/dart_package_template?logo=dart)](https://pub.dev/packages/dart_package_template/score)
[![likes](https://img.shields.io/pub/likes/dart_package_template.svg)](https://pub.dev/packages/dart_package_template/likes)
[![popularity](https://img.shields.io/pub/popularity/dart_package_template.svg)](https://pub.dev/packages/dart_package_template/popularity)

## ✨ Features
- Ready for immediate package publication to [pub.dev](https://pub.dev/).
- Pre-configured `pubspec.yaml` with recommended fields.
- Multiple example projects in the `example/` directory.
- Linting setup with `lints` package for code quality, following the [Effective Dart](https://dart.dev/guides/language/effective-dart) style guide.
- (Recommended) [MPL-2.0 License](https://opensource.org/licenses/MPL-2.0) for open source projects.
- Unit tests setup with `test` package.
- GitHub Actions workflows for automated testing/QA jobs on push events and PRs.

This repository is also published as a package on [pub.dev](https://pub.dev/packages/dart_package_template) to make sure it's always kept up to date on the most recent best practices 🫶

## 🔮 Getting Started

1. **Create a new repository**
    - Click the "Use this template" button on the GitHub page for this repository.
    - Fill in the details for your new repository and create it.
        - **🛑✋ IMPORTANT!** Make sure to name your new repository and package with underscore separators, **`just_like_this`** as required by Dart.
2. **Clone your new repository**
    ```bash
    git clone <your-repo-url>
    cd <your-repo-name>
    ```
3. **Update `pubspec.yaml`**
    - Change the `name`, `description`, `homepage`, `repository`, and `issue_tracker` fields to match your package.
    - Update the `environment` SDK constraints if necessary.
    - Update the same fields in `example/pubspec.yaml`.


