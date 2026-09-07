# Firebase Rules Record

Last verified: 2026-09-07
Firebase project: `scienceinonepiecep3-4`
Database: Cloud Firestore `(default)`

## Incident

The original Firestore Test Mode rule expired on 2026-06-05. After expiry, all client requests were denied and the online leaderboard stopped working.

## Deployed policy

Collection: `science_eastblue_lb/{player}`

- Public read is allowed for the in-game leaderboard.
- Create requires `name`, `score`, and `ts`.
- The stored `name` must equal the document ID.
- `name` must be a string.
- `score` must be numeric and non-negative.
- Updates must preserve the player identity and cannot reduce the score.
- Delete is denied because no delete rule is granted.
- The rule has no Test Mode expiry date.

## Verification

- Firebase Console: rules were published by the project owner.
- Client-access check: the Firestore REST endpoint returned HTTP 200 and an existing `science_eastblue_lb` document after publication.
- The `main`/`data` branch relationship was not changed.
- The production HTML and question-bank files were not changed.
