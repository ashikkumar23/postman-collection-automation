# Postman Report

[![Actions Status](https://github.com/ashikkumar23/postman-reports/workflows/Newman%20Tests/badge.svg)](https://github.com/ashikkumar23/postman-reports/actions/workflows/github-actions-htmlextra-report.yml)

This repo shows how to run `Postman` collection using `Newman` within the `GitHub Actions` job and generate the `htmlextra` test results report

## 🚀 Description:
- `Newman` is a command-line collection runner for `Postman`
- `Newman` allows you to effortlessly run and test a `Postman` collection directly from the command-line
- `Newman` is built with extensibility in mind so that you can easily integrate it with your continuous integration servers and build systems

## 🚀 Steps:
- Download and Install [Postman](https://www.postman.com/downloads/)
- Create a new `Collection` and save your requests in a collection for reuse and sharing
- Create a new `Environment` and save values you frequently use in an environment
- Export the newly created `Collection` along with the `Environment` from `Postman` to your local directory
- Add the `postman_collection` and `postman_environment` to the newly created `GitHub` repo
- Create a `GitHub Actions` workflow ( i.e., `.github/workflows/github-actions-htmlextra-report.yml` ) to run `postman collection` using `Newman` and generate `test report` via `html extra reporter`
- Upon every `push` and `pull_request`, the workflow would be triggered with `Artifacts` produced during runtime ( i.e., `test-run-reports` ) that contain the html report ( i.e., `test_report.html` )
- Or, the simplest way is to fork the repository https://github.com/ashikkumar23/postman-reports, make a small change and push the changes to see workflow getting triggered with the generation of html report ( i.e., `test_report.html` )