Code Review Checklist
===========================================

> A hardly exhaustive collection of considerations when peer-reviewing software.

- - -

Clean, merge-ready pull requests:

##### Functionality

  - [ ] implement relevant specification(s)
  - [ ] anticipate and address failure modes
  - [ ] avoid (or adequately justifies) obvious performance issues
  - [ ] provide appropriate user feedback
  - [ ] expose logs, errors, and other runtime debugging details as needed

##### Testing

  - [ ] secure behaviors described in relevant specification(s)
  - [ ] test public interfaces
  - [ ] cover anticipated failure modes
  - [ ] benchmark recognized performance issues
  - [ ] run green

##### Legibility

  - [ ] embrace style and patterns established by the project, team, and
      community
  - [ ] consume existing libraries, methods, and types
  - [ ] use suggestive names for functions, variables, and classes
  - [ ] document public interfaces as appropriate

##### Security

  - [ ] bound and sanitize inputs
  - [ ] sanitize outputs, including analytics and [logs][sanitize-logs]
  - [ ] recognize and address common vulnerabilities ([SQL
      injection][sql-injection], [XSS][xss], [buffer overruns][buffer-overflow],
      etc)
  - [ ] isolate platform-/environment-specific functionality

##### VCS Hygiene

  - [ ] provide [clear, useful commit messages][git-commit]
  - [ ] [reference external issues, tickets, and bugs][supplemental-docs] where
      they exist
  - [ ] use incremental, atomic commits
  - [ ] avoid binaries, logs, local configurations, environment-specific files,
      plaintext secrets, or other unwanted artifacts

##### License

[MIT](LICENSE) licensed - fork, contribute, and enjoy!

[git-commit]: http://chris.beams.io/posts/git-commit/
[supplemental-docs]: https://rjzaworski.com/2015/05/supplemental-documentation
[sql-injection]: https://www.owasp.org/index.php/SQL_Injection
[xss]: https://www.owasp.org/index.php/XSS
[buffer-overflow]: https://www.owasp.org/index.php/Buffer_Overflow
[sanitize-logs]: https://www.owasp.org/index.php/Logging_Cheat_Sheet#Data_to_exclude
