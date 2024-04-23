# Conventional Commits for Enhanced Clarity

To make sure our commit messages are clear and follow a common format, it's important to use a consistent approach. These messages hold important information that helps us keep track of what we're doing, decide which changes to use in different parts of our project, and even create things like updates and logs automatically. [Conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) help us build a complete history of our changes that's easy for people and computer programs to understand.

## Commit Formats

```xml
<type>[optional scope]: <description>
```

### Examples of Commit Formats

- **`feat(auth): implement user authentication`**
- **`fix: resolve button alignment issue`**

## Commit Types (Mandatory)

- **build**: This MUST be used when changes affect build components like tools, external dependencies, dev dependencies, and similar elements. For instance, in Node.js projects, tools such as linters or formatters MUST NOT be updated without generating new releases or changes in the app.
    
    Example: **`build(dependencies): update webpack to version 5`**
    
- **chore**: This MUST be used when there are changes in files such as .gitignore, .env, yaml, toml, or package.json (adding or removing information but not dependencies or scripts), or when adding comments in any type of files, even in the source code.
    
    Example: **`chore(.gitignore): add build artifacts to gitignore`**
    
- **ci**: This MUST be used when there are changes in scripts or configuration files focused on the CI or CD process.
    
    Example: **`ci(pipeline): update deployment script`**
    
- **deprecate**: This MUST be used when an existing functionality will be deprecated, but any kind of source code MUST NOT be removed because it will continue working, providing some feature. For instance, old public APIs MAY get deprecated because newer, more efficient APIs are available.
    
    Example: **`deprecate(api): mark legacy endpoint as deprecated`**
    
- **docs**: This MUST be used when there are changes in the documentation stored in the repository (additions, updates, improvements, or removals).
    
    Example: **`docs(readme): update installation instructions`**
    
- **feat**: This MUST be used when implementing a new feature in the application. A BREAKING CHANGE is indicated when feat begins with an exclamation mark (!), as in !feat. This type will generate a new major version of the software.
    
    Example: **`feat(auth): add social media login options`**
    
- **fix**: This MUST be used when fixing a defect (bug) in the application.
    
    Example: **`fix(ui): correct navigation bar rendering`**
    
- **perf**: This MUST be used when making improvements in performance (time execution, memory consumption, or similar) that do not affect the behavior or change an existing feature.
    
    Example: **`perf(api): optimize database query`**
    
- **refactor**: This MUST be used when a piece of code changes to improve its legibility or for following best practices (formatting, clean code, applying design patterns, and so on). However, it MUST NOT fix a bug, add a feature, or affect/alter existing behavior in the software.
    
    Example: **`refactor(util): simplify date formatting function`**
    
- **remove**: This MUST be used when a feature has been removed, typically features that are deprecated and need to be removed completely. This constitutes a breaking change, and it will generate a significant change in semantic versioning.
    
    Example: **`remove(deprecated): delete legacy API endpoints`**
    
- **revert**: This MUST be used to revert commits that were previously merged to the main branch because they are causing serious problems or were just accidentally merged into the main branch.
    
    Example: **`revert: revert accidental merge of feature branch`**
    
- **security**: This MUST be used to add security improvements or resolve reported/found security issues.
    
    Example: **`security(auth): patch vulnerability in authentication`**
    
- **style**: This MUST be used when the source code will be updated with changes such as adding white-spaces, formatting, adding missing semi-colons, and so on, but it MUST NOT otherwise change the implementations.
    
    Example: **`style(ui): format code according to style guide`**
    
- **test**: This MUST be used when there are enhancements, additions, revisions, or changes to the suite of automated tests for the software.
    
    Example: **`test(unit): add unit tests for user validation`**
    
- **push**: This MAY be used when some tools are generated as libraries or even Docker containers, and those need to be published/pushed to some service, such as Code Artifact, Nuget, GitHub, DockerHub, and so on.
    
    Example: **`push(library): publish library to Code Artifact`**
    
- **deploy**: This MAY be used when it is important to generate a deployment manually without waiting for some changes in source code.
    
    Example: **`deploy(staging): manually deploy the latest changes`**
    
- **rollback**: This MAY be used when a software rollback is obligatory.
    
    Example: **`rollback(production): roll back to previous stable version`**
    
- **ops**: This MUST be used when source code changes are focused on infrastructure but MUST NOT affect the source code of the software.
    
    Example: **`ops(terraform): update infrastructure configuration`**
    
- **release**: This MAY be used to generate manual releases when necessary.
    
    Example: **`release: create v2.0.0 release`**
    
