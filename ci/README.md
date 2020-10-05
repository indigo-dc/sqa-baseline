# Continuous integration tools

[![Build Status](https://travis-ci.org/indigo-dc/sqa-baseline.svg?branch=master)](https://travis-ci.org/indigo-dc/sqa-baseline)

This directory contains tools and files for continuous integration (CI).
Specifically, [`deploy.sh`](deploy.sh) runs on successful `master` branch builds that
are not pull requests.
The contents of `../webpage` are committed to the `gh-pages` branch.
The contents of `../output` are committed to the `output` branch.

For more information on the CI implementation, see the CI setup documentation in `SETUP.md`.
