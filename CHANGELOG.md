## [1.1.7] - 04/03/2020
- Pass scenario tags into scenerio level hooks to allow for custom actions - this is a breaking changed to the `Hook` interface and hook implementations will need to be updated to cope with the extra parameter

## [1.1.6+4] - 03/02/2020
- Fixed issue with empty cells in scenario table parameters
- Fixed issue with a leading comment in feature files

## [1.1.6+3] - 14/01/2020
- Fixed issue with scenerio not being parsed correctly when under a scenario outline in the same feature file

## [1.1.6+2] - 13/01/2020
- Fixed issue with non-capturing regex groups in step patterns and made the well known pluralisation parameter '(s)' a non-capturing regex group

## [1.1.6+1] - 10/01/2020
- Ensured aysnc errors when executing a scenario do not cause the whole test run to crash from an unhandled exception or error - each scenario is now run in its own zone

## [1.1.6] - 10/01/2020
- Ensured aysnc errors when executing a scenario do not cause the whole test run to crash from an unhandled exception - each scenario is now run in its own zone
- Surfaced library exception types

## [1.1.5+2] - 07/01/2020
- Ensured stack traces are propogated when an error occurs during test execution
- Fixed error with message from GherkinStepNotDefinedException that would include the Gherkin keyword in the example regex pattern

## [1.1.5+1] - 24/12/2019
- Require Dart 2.3.0 or greater
- Fixed various analysis errors

## [1.1.5] - 05/12/2019
- Fixed lint errors

## [1.1.4] - 05/12/2019
- Allowed comments at the end of a table line
- Moved `onBeforeScenario` hook to run after the scenerio world has been created to allow the hook to access the world

## [1.1.3] - 27/09/2019
- Relaxed constraint on the test lib

## [1.1.2] - 22/09/2019
- Fixed issue with scenerio outline name being reported incorrectly

## [1.1.1] - 22/09/2019
- Added `asMap` helper method to a table so a table can be represented as a map to help with serialisation to types

## [1.1.0] - 20/09/2019
* Implemented langauges - features can now be written in different languages / dialects! See https://cucumber.io/docs/gherkin/reference/#overview for supported dialects.

## [1.0.12] - 18/09/2019
* Fixed version constraint analysis errors

## [1.0.11] - 18/09/2019
* Fixed path dependency to be backwards compatible with flutter_driver

## [1.0.10] - 18/09/2019
* Updated test dependency

## [1.0.9] - 16/09/2019
* Fixed issue where tags were not allowed on features
* Refactor of the way tags are handled so they are inherited by children if requried (see https://cucumber.io/docs/cucumber/api/#tag-inheritance)
* Fixed the JSON reporter so that is adheres to to the cucumber json reporter spec.

## [1.0.8] - 13/09/2019
* Fix an issue where line terminators where not allowed in well known {string} parameters

## [1.0.7] - 25/08/2019
* Fix path dependency resolution

## [1.0.6] - 25/08/2019
* Added 'Scenario Outline' and 'Example' functionality (see: example/features/calculator_scenerio_outline_example.feature)
* Fixed issue with parsing a negative number when using the '{num}' parameter in a step

## [1.0.5] - 23/08/2019
* Fixed complex co-variant issue with step code definitions
* Fixed parsing issue when Background block has no name

## [1.0.4] - 11/07/2019
* Fix for dart analysis covariance complaints with step definition input generic types

## [1.0.3] - 20/06/2019
* Fix dependencies conflict with flutter_test and flutter_driver

## [1.0.2] - 20/06/2019
* Updated dependencies

## [1.0.1] - 20/06/2019
* Added the ability to add attachments which gives the ability to set screenshots or other data against the scenerio
* Added before & after hooks for step execution

## [1.0.0] - 04/06/2019
* Fixed throw Error sub types not getting handle properly and halting test execution fixes https://github.com/jonsamwell/dart_gherkin/issues/2
* Fixed linter warnings
* Made v1 release as api's are stable

## [0.0.4] - 23/04/2019
* Exported missing step and process classes
* Added JSON reporter that can be use to generate HTML reports (PR from @Holloweye)

## [0.0.3] - 15/03/2019
* Fixed up more issues with pubspec.yaml

## [0.0.2] - 15/03/2019
* Fixed up issues with pubspec.yaml

## [0.0.1] - 15/03/2019
* Migration of core Gherkin code from flutter_gherkin package (https://github.com/jonsamwell/flutter_gherkin) so there is not Flutter specific dependencies on the core Gherkin functionality.
