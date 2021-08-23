# Changelog


## 2021-04-07
- Implement proper cleanup of resources when the process receives SIGTERM

## 2021-04-07
- Remove the temporary debug endpoint before the release

## 2021-05-07
- Refactor exports so the public API is clearer and easier to use

## 2021-05-13
- Simplify the build script by using the same steps for dev and prod

## 2021-05-31
- Simplify the config validation by using a declarative schema

## 2021-06-18
- Handle the case when the external service returns an empty list

## 2021-06-30
- Clean up the TODO comments that were already addressed

## 2021-06-30
- Bump the Docker base image to get the latest security patches

## 2021-07-06
- Support both YAML and JSON config formats for flexibility

## 2021-07-06
- Handle edge case when the response body is empty but status is 200

## 2021-07-06
- Correct the default value for the feature flag in production

## 2021-07-18
- Update dependencies and resolve compatibility warning from pytest

## 2021-07-30
- Refactor the parser to use a proper state machine instead of regex

## 2021-07-30
- Add a note in the README about the breaking change in 2.0

## 2021-08-05
- Fix bug where the parser would hang on malformed input

## 2021-08-11
- Handle the case when the config file exists but is not readable

## 2021-08-17
- Clean up the TODO comments that were already addressed

## 2021-08-23
- Improve the error recovery when the database connection is lost
