# CHANGELOG

## Unreleased
* Docker

## 0.1.6 (2020-07-10)
UI:
* Definitions for Risk types are now available via Popovers. Fixes #66
* Renamed "Group", "User", "Role" as "Inline Group Policy", "Inline User Policy", and "Inline Role Policy" respectively. Addresses #63
* Fixes links to the inline policies in case there are duplicate names. Addresses #63
* Moves "Attached to Principal(s)" to the Finding card instead of in the finding details in case there are duplicate policy names. Fixes #63

## 0.1.5 (2020-07-08)
* Made callable via script to partially fix #39
* Move to virtualenv instead of Pipenv

## 0.1.4 (2020-05-26)
* Inline policies are now clearly mapped to their roles.

## 0.1.3 (2020-05-16)
* Excel/CSV export capability
* Table row selection capability

## 0.1.2 (2020-05-14)
Just a few UI fixes:
* Sort columns in Summary table by searching.
* Reasonable size restrictions on "services affected" columns, with Scrollable cells

## 0.1.1 (2020-05-12)
* Bug fix: issue where "Data Exfiltration" count was showing up in the "Resource Exposure" count column in the IAM Principals tab
* Added "Attached to Principals" dropdown card for Customer-Managed and AWS-Managed Policies

## 0.1.0 (2020-05-11)
* Granular exclusions: Fixed issue where exclusions file was including dangling policies in the results (Fixes #33)
* Changed IAM Principals table so that the principals can be sorted according to their risks. This will really help with pentesting

## 0.0.14 (2020-05-07)
* Fix issue where Data Exposure tallies were not showing up in the AWS Managed table correctly.

## 0.0.13 (2020=05-07)
* Windows compatibility fixes

## 0.0.12 (2020-05-07)
* Various UI improvements, like sortable tables. Fixes #22. See https://opensource.salesforce.com/cloudsplaining/ for the latest example.
* Fixes #27 - issue arising from where "expanded_actions" is empty

## 0.0.11 (2020-05-06)
* Fixed an issue arising from policies where "Deny" was used in effect with no resource constraints. Fixes #23.

## 0.0.10 (2020-05-05)
* Removed the recursive credentials method from the `download` command.
* Fixed occasional installation error occurring from outdated Policy Sentry versions.
* Fixed instructions for the `download` command.

## 0.0.9 (2020-05-03)
* HTML report now always shows Trust Policies for Roles, even if they do not allow assumption from a Compute Service. This can help assessors with triaging and pentesters for targeting.

## 0.0.8 (2020-05-03)
* Migrated to GitHub actions with automated Homebrew releases

## 0.0.7 (2020-05-03)
* Added separate tab for IAM Principals
* HTML Report improvements - using tabs now
* Changed the naming of some objects to make the object naming more in line with the AWS IAM API Data Types. https://docs.aws.amazon.com/IAM/latest/APIReference/API_Types.html

## 0.0.6 (2020-05-01)
* Fix `exclude-actions` in the exclusions file - it was not being respected before.
* Add a recursive scanning option.

## 0.0.4 (2020-05-01)
* Provide option to skip opening HTML report (`--skip-open-report`)
* Provide report indicator on whether it is assumable by compute services
* Dropdown menu for report

## 0.0.2 (2020-04-30)
* Quick markdown bug fix

## 0.0.1 (2020-04-30)
* Open sourced!
