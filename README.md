Code Review Checklist
===========================================

A hardly exhaustive collection of reminders that clean, merge-ready pull
requests:

Legibility
-------------------------------------------

  - [ ] reinforce patterns esablished by the project, team, and community
  - [ ] follow style guidelines
  - [ ] reuse existing libraries, methods, and types
  - [ ] use suggestive names for functions, variables, and classes
  - [ ] document public interfaces (if required)

Functionality
-------------------------------------------

  - [ ] implement the spec
  - [ ] anticipate and handles failure modes
  - [ ] avoid (or adequately justifies) obvious performance issues
  - [ ] provide appropriate feedback to the user
  - [ ] expose logs, errors, and other runtime debugging details as needed

Testing
-------------------------------------------

  - [ ] test public interfaces at an appropriate level
  - [ ] cover anticipated failure modes
  - [ ] run green

Security
-------------------------------------------

  - [ ] sanitize inputs
  - [ ] sanitize outputs, including analytics and logs
  - [ ] recognize and address common vulnerabilities (SQL injection, XSS,
      buffer overruns, etc)
  - [ ] isolate platform-/environment-specific functionality

VCS Hygiene
-------------------------------------------

  - [ ] provide a commit message with a clear, useful description
  - [ ] reference external issues, tickets, and bugs as needed
  - [ ] use incremental, atomic commits
  - [ ] avoid binaries, logs, local configurations, or other unwanted artifacts

License
-------------------------------------------

[MIT](LICENSE) licensed - fork, contribute, and enjoy!

