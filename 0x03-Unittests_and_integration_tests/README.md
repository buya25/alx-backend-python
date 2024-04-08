# Project Readme

This project consists of a series of unit tests and integration tests for a Python codebase. The tests are structured into different tasks, each focusing on a specific aspect of testing.

## Required Files

The following files are required for this project:

- `utils.py`: Contains utility functions to be tested.
- `client.py`: Contains classes related to HTTP client functionality.
- `fixtures.py`: Contains fixtures used in integration tests.

## Tasks

### 0. Parameterize a unit test

- **Description**: Implement unit tests for the `utils.access_nested_map` function.
- **Test Class**: `TestAccessNestedMap`
- **Inputs to Test**: Various nested map structures and paths
- **Expected Behavior**: Ensure the function returns the expected result for different inputs.

### 1. Parameterize a unit test

- **Description**: Implement unit tests for handling exceptions in `utils.access_nested_map`.
- **Test Class**: `TestAccessNestedMap`
- **Inputs to Test**: Nested map structures and paths causing KeyError
- **Expected Behavior**: Ensure the function raises KeyError and the exception message is as expected.

### 2. Mock HTTP calls

- **Description**: Test `utils.get_json` function without making actual HTTP calls.
- **Test Class**: `TestGetJson`
- **Inputs to Test**: Various URLs and expected payloads
- **Expected Behavior**: Ensure `get_json` returns the expected result and does not make actual HTTP calls.

### 3. Parameterize and patch

- **Description**: Test memoization behavior using the `utils.memoize` decorator.
- **Test Class**: `TestMemoize`
- **Inputs to Test**: Invocation of a method multiple times
- **Expected Behavior**: Ensure the method is only called once due to memoization.

### 4. Parameterize and patch as decorators

- **Description**: Test `client.GithubOrgClient` class without making actual HTTP calls.
- **Test Class**: `TestGithubOrgClient`
- **Inputs to Test**: Different organization names
- **Expected Behavior**: Ensure the `org` method returns the correct value without making external HTTP calls.

### 5. Mocking a property

- **Description**: Test `_public_repos_url` property of `client.GithubOrgClient` class.
- **Test Method**: `test_public_repos_url`
- **Expected Behavior**: Ensure the property returns the expected URL based on mocked payload.

### 6. More patching

- **Description**: Test `public_repos` method of `client.GithubOrgClient` class.
- **Test Method**: `TestGithubOrgClient.test_public_repos`
- **Expected Behavior**: Ensure the method returns the expected list of repositories and is called once.

### 7. Parameterize

- **Description**: Test `has_license` method of `client.GithubOrgClient` class.
- **Test Method**: `TestGithubOrgClient.test_has_license`
- **Inputs to Test**: Different repositories and license keys
- **Expected Behavior**: Ensure the method returns the expected value based on repository and license key.

### 8. Integration test: fixtures

- **Description**: Integration test for `client.GithubOrgClient.public_repos` method.
- **Test Class**: `TestIntegrationGithubOrgClient`
- **Inputs to Test**: Various fixtures containing example payloads
- **Expected Behavior**: Ensure the method returns the expected results based on mocked requests.

### 9. Integration tests

- **Description**: More integration tests for `client.GithubOrgClient.public_repos` method with additional scenarios.
- **Test Methods**: `test_public_repos`, `test_public_repos_with_license`
- **Expected Behavior**: Ensure the method returns the expected results based on fixtures and scenarios.
