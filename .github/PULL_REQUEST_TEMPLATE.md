## Related Tickets & Documents
- https://repam.atlassian.net/browse/TK-XXX

## What type of PR is this? (check all applicable)
- [ ] 🍕 Feature
- [ ] 🐛 Bug Fix
- [ ] 📝 Documentation Update
- [ ] 🎨 Style
- [ ] 🧑‍💻 Code Refactor
- [ ] 🔥 Performance Improvements
- [ ] ✅ Test
- [ ] 🤖 Build
- [ ] 🔁 CI

## Mobile & Desktop Screenshots/Recordings

<!-- Visual changes require screenshots -->

## Steps to QA
<!--
1. Click a link
2. Do this thing
3. ....
4. Validate you see the thing working
-->

## Avoid regression
E2E tests are triggered manually on each environment. Please make sure to run the tests before merging the PR.

To run the tests, execute the following command:
```bash
curl -X POST "https://drone.repamtech.fr/api/repos/REPAM-TECH/e2e/builds?branch=&{REPO_NAME=<repo_name>}&{ENVIRONMENT=dev}" \\n  -H "Authorization: Bearer <drone_token>"
```
Or by using [repamflow](https://www.npmjs.com/package/@repam-tech/repamflow)
