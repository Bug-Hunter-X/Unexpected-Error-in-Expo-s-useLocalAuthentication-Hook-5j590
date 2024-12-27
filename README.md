# Unexpected Error in Expo's useLocalAuthentication Hook

This repository demonstrates a bug in Expo's `useLocalAuthentication` hook where an unexpected error occurs when the authentication process is canceled. The default `cancelable: true` behavior, while useful, lacks robust error handling, making it difficult to manage unexpected interruptions.

The `useLocalAuthBug.js` file showcases the problem: the hook throws an error without providing enough context on why authentication failed.  `useLocalAuthSolution.js` demonstrates a solution with improved error handling.

## Reproducing the Bug

1. Clone this repository.
2. Run `expo start`.
3. Observe the error message when the authentication process is canceled.