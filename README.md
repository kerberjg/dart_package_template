<div align="center">

<!-- template:in
# ${package_name}
${package_description}
 /template:in -->
<!-- template:out -->
# dart_package_template
GitHub template repository for Dart packages, ready for pub.dev publication.
<!-- /template:out -->


<!-- template:in
```bash
dart pub get ${package_name}
```
 /template:in -->
<!-- template:out -->
```bash
dart pub get dart_package_template
```
<!-- /template:out -->

<!-- Badges -->

<!-- template:in
[![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](LICENSE)
[![build](https://github.com/${github_username}/${repo_name}/actions/workflows/package.yaml/badge.svg)](https://github.com/${github_username}/${repo_name}/actions/workflows/package.yaml)
[![example](https://github.com/${github_username}/${repo_name}/actions/workflows/example.yaml/badge.svg)](https://github.com/${github_username}/${repo_name}/actions/workflows/example.yaml)
[![stars](https://img.shields.io/github/stars/${github_username}/${repo_name}.svg)](https://github.com/${github_username}/${repo_name}/stargazers)
<br/>
[![pub package](https://img.shields.io/pub/v/${package_name}?logo=dart)](https://pub.dev/packages/${package_name})
[![pub score](https://img.shields.io/pub/points/${package_name}?logo=dart)](https://pub.dev/packages/${package_name}/score)
[![likes](https://img.shields.io/pub/likes/${package_name}?logo=dart)](https://pub.dev/packages/${package_name}/likes)
 /template:in -->
<!-- template:out -->
[![License: MPL 2.0](https://img.shields.io/badge/License-MPL_2.0-brightgreen.svg)](LICENSE)
[![build](https://github.com/kerberjg/dart_package_template/actions/workflows/package.yaml/badge.svg)](https://github.com/kerberjg/dart_package_template/actions/workflows/package.yaml)
[![example](https://github.com/kerberjg/dart_package_template/actions/workflows/example.yaml/badge.svg)](https://github.com/kerberjg/dart_package_template/actions/workflows/example.yaml)
[![stars](https://img.shields.io/github/stars/kerberjg/dart_package_template.svg)](https://github.com/kerberjg/dart_package_template/stargazers)
<br/>
[![pub package](https://img.shields.io/pub/v/dart_package_template?logo=dart)](https://pub.dev/packages/dart_package_template)
[![pub score](https://img.shields.io/pub/points/dart_package_template?logo=dart)](https://pub.dev/packages/dart_package_template/score)
[![likes](https://img.shields.io/pub/likes/dart_package_template?logo=dart)](https://pub.dev/packages/dart_package_template/likes)
<!-- /template:out -->

</div>

### 💙 Use cases
- 🏝️ **A weekend project**: quickly start a new OSS Dart project with everything set up
- 📚 **Learning**: understand best practices for Dart package structure, linting, testing, and CI
- 💻 **Production-ready boilerplate**: complete starting point for a high-quality Dart package


## ✨ Features
- Unopinionated! A minimal example focused on compliance with Dart guidelines
- Ready for immediate package publication to [pub.dev](https://pub.dev/)
- Pre-configured `pubspec.yaml` with recommended fields
- Multiple example projects in the `example/` directory
- Linting setup with `lints` package for code quality, following the [Effective Dart](https://dart.dev/guides/language/effective-dart) style guide
- (Recommended) [MPL-2.0 License](https://opensource.org/licenses/MPL-2.0) for open source projects
- Unit tests setup with `test` package
- GitHub Actions workflows for automated testing/QA jobs on push events and PRs
- GitHub issues/PR templates

This repository is also published as a package on [pub.dev](https://pub.dev/packages/dart_package_template) to make sure it's always kept up to date on the most recent best practices 🫶

#### Coming up next:
- **CLI utility** for maintenance/updates (separate repo/package)

---

## 🔮 Usage Guide

### Getting Started

1. **Create a new repository**
    - Click the "Use this template" button on the GitHub page for this repository.
    - Fill in the details for your new repository and create it.
        - **🛑✋ IMPORTANT!** Make sure to name your new repository and package with underscore separators, **`just_like_this`** as required by Dart.
2. **Clone your new repository**
    ```bash
    git clone <your-repo-url>
    cd <your-repo-name>
    ```
3. **Run `./init` script**
    - **🛑✋ IMPORTANT!** Do not skip this step
    - This will set the correct names, descriptions and URLs in all relevant files (`pubspec.yaml`, `README.md`, GitHub workflows, etc.) based on your repository name and details
4. **Update `README.md`**
    - We recommend you keep the sections, titles and the structure of this README as-is
    - Update the content to reflect your package's purpose, features, and usage
5. (optional) **Update `LICENSE`**
    - We recommend the included [`MPL-2.0 License`](https://opensource.org/licenses/MPL-2.0) for open source packages, as it's business-friendly and allows for both open source and proprietary use
    - If you choose a different license, make sure to update the `LICENSE` file accordingly

### Development & Maintenance

1. Make sure you have the following enabled in your IDE:
    - Dart SDK
    - Dart/Flutter Linting
    - "Format on Save"
2. **Write your code!** implement your package functionality in `lib/`, however you like 💙
    - Make sure there are no format/analysis issues reported by your IDE!
3. **Update & run tests** to ensure everything is working as expected:
    ```bash
    dart test
    ```
4. **Commit & push your changes** to your repository. We recommend using a standardized branching strategy (such as [`GitFlow`](https://nvie.com/posts/a-successful-git-branching-model/)) and maintaining a cohesive commit message/history style.

5. **Create a Pull Request** to merge your changes into the `main` branch.
    - Make sure all **GitHub Actions** checks pass before merging
    - Once approved, merge the PR into `main`

6. **Review & Refine**
    - Regularly review your codebase for improvements, refactoring, and updates to dependencies
    - Keep your documentation up to date in `README.md` and `CHANGELOG.md`


### Publishing

1. **Commit the version bump**
    - Update the version in `pubspec.yaml` according to [Semantic Versioning](https://semver.org/)
    - Update the `CHANGELOG.md` with the changes made in this version
        - 🤫 _psst!_ you can use [git log](https://git-scm.com/docs/git-log) command to help you with this, such as `git log --oneline --decorate 1.0.0..HEAD` to see all commits since version 1.0.0
    - Name the commit something like `Bump version to x.y.z`
    - Create a git tag for the new version: `git tag x.y.z`

2. **Publish to pub.dev**
    - **IMPORTANT:** Make sure you have an account on [pub.dev](https://pub.dev/) and are logged in via the command line using `dart pub login`
    - First run `dart pub publish --dry-run` to ensure everything is ready for publication
    - If the above command reports any issues, address them before proceeding
    - When ready, run `dart pub publish` to publish your package

### Next steps

- Share your work! Announce your package on social media, relevant forums, and communities to gain users and feedback.
- Invite collaborators! Open your repository to contributions from others to help improve and maintain the package.
- Keep learning and improving! Regularly update your package with new features, bug fixes, and improvements based on user feedback.

---

**That's it! 🥳 Congratulations on starting the journey of creating your Dart package!** 🎉🤗💙

The Dart/Flutter community is made better by contributions like yours. Make sure to reach out and engage with others in the community, share experiences with other devs,  and keep building amazing things!

>
> Our community is warm and welcoming, make sure to act within that spirit! 💖
> 

---

## 📄 License

This project is licensed under the Mozilla Public License 2.0 - see the [LICENSE](LICENSE) file for details.

## 🔥 Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes. Make sure to read the following guidelines before contributing:

- [Code of Conduct](CODE_OF_CONDUCT.md)
- [CONTRIBUTING.md](CONTRIBUTING.md)
- ["Effective Dart" Style Guide](https://dart.dev/guides/language/effective-dart)
- [**pub.dev** Package Publishing Guidelines](https://dart.dev/tools/pub/publishing)

## 🙏 Credits & Acknowledgements

### Contributors 🧑‍💻💙📝

This package is developed/maintained by the following rockstars!
Your contributions make a difference! 💖

<!-- template:in
![contributors badge](https://readme-contribs.as93.net/contributors/${github_username}/${repo_name}?textColor=888888)
 /template:in -->
<!-- template:out -->
![contributors badge](https://readme-contribs.as93.net/contributors/kerberjg/dart_package_template?textColor=888888)
<!-- /template:out -->

### Sponsors 🫶✨🥳

Kind thanks to all our sponsors! Thank you for supporting the Dart/Flutter community, and keeping open source alive! 💙

<!-- template:in
![sponsors badge](https://readme-contribs.as93.net/sponsors/${github_username}?textColor=888888)
 /template:in -->
<!-- template:out -->
![sponsors badge](https://readme-contribs.as93.net/sponsors/kerberjg?textColor=888888)
<!-- /template:out -->

---

<!-- Keep the below notice -->

<div align="center">

> Based on [`dart_package_template`](https://github.com/kerberjg/dart_package_template) - a high-quality Dart package template with best practices, CI/CD, and more! 💙✨

</div>