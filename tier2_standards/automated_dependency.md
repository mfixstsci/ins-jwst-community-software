# Project Must Use an Automated Dependency Update Tool

This is one of the tier 2 standards. See full list [on the main page](../README.md).

## Short description

Automated dependency update tools automatically detect which of the third-party software dependencies are out of date in your project's software environment, and automatically open a Pull Request with proposed changes to update said dependencies.  These tools help prevent security vulnerabilities and make developers aware of new updates to dependencies, which may come with new, useful features.

## Importance of this standard

Automated dependency update tools help ensure that your software is up-to-date with latest third-party dependencies (e.g. `numpy`, `astropy`, `pytest`, etc.), thus helping your software to continue to be maintainable as the python software ecosystem evolves.  Furthermore, these tools help ensure that your software is not susceptible to security vulnerabilities (which is especially important for web applications).  Lastly, having periodically-updated dependencies ensures that your software continues to be installable and operational by external users who may be using fresh software environments and installations.

## Options for this standard

While there are a number of options available, we recommend [`dependabot`](https://dependabot.com/), which is native to GitHub (and thus free for all repositories), or [`pyup`](https://pyup.io) (free for public repositories).

## How to apply this standard

- For `dependabot`, visit https://app.dependabot.com/auth/sign-up,  and follow the instructions to create an account and add your specific software repository.
- For `pyup`, visit https://pyup.io/, and follow the instructions to create an account and add your specific software repository.

## Useful Links

- The `jwql` repository serves as an example of a project using `pyup`.  See the [`jwql` `pyup.yml` configuration file](https://github.com/spacetelescope/jwql/blob/develop/.pyup.yml) as an example of a configuration file.
