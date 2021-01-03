# Building a CI/CD Pipeline

In this text, I assume that the application would be built with __Python__.

## Tools for Different Steps

### Linting

Linter is a tool for analysing source code to flag programming errors, bugs, stylistic errors, and suspicious constructs. Most popular linter for Python is probably __Pylint__. Also __Flake8__, __Pylama__ and __mypy__ have been recommended on certain sites.

Linting may also cover other parts such as CSS files (for instance, __Stylelint__) or documentation (for instance, __Markdownlint__).

### Testing

There is a built-in test runner in the Python standard library called __unittest__. Other popular test runners include __nose__ (or __nose2__) and __pytest__.

Also many online testing tools are available, but in CI/CD environments, the above mentioned tools may be more handy.

## Self-hosted or Cloud-based Environment?

Nowadays, a cloud-based CI/CD setup is probably the default choice. It makes setupping the CI environment more straightforward if you do not have any special requirements related to your product. For smaller projects, it is usually also cheaper and you don’t have to worry so much upon maintaining the environment.

Self-hosted setup may, however, be the right choice if you have more specialised needs on top of generally used default environments. The same applies if you need more resources (CPU time, memory, etc.) or if your project is large or if, for instance, multiple teams in a larger company needs similar CI/CD setup.
