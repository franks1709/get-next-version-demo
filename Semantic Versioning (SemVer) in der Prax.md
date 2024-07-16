Semantic Versioning (SemVer) in der Praxis + GitHub Action    deutsch
=====================================================================

x.y.z

major: Breaking Change
minor: Neue Feature (abwärtskompatibel)
patch: Bugfixes, Fehlerbehebung, …


5.17.0

5.17.1		==> Update unproblematisch
5.18.0		==> Update unproblematisch
6.0.0		==> Update eventuell problematisch


Conventional commits:
feat: Implement user registration.
fix: Fix typo in registration form.
feat!: Reject non-authenticated users.
chore: Remove some comments.
docs: Update README-md.
refactor: Rewrite user authentication code.

5.17.0 => chore => chore => chore 	5.17.0
5.17.0 => chore => fix => chore		5.17.1
5.17.1 => fix => chore => feat		5.18.0
5.18.0 => chore => feat! => fix		6.0.0
